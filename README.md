# 🌐 Redes de Computadores – Guia Completo 🌐

![Redes Banner](https://img.shields.io/badge/Networking-Essential-blue?style=for-the-badge)

---

## 📌 O que são Redes de Computadores?

Uma **rede de computadores** é um conjunto de dispositivos conectados que compartilham **dados, recursos e serviços** entre si.  
Elas são essenciais para comunicação, armazenamento e gerenciamento de informação no mundo digital.

- 💻 Conexão entre dispositivos  
- 🌍 Compartilhamento de dados e recursos  
- 🛡️ Base para segurança e monitoramento  

---

## 🛠 Tipos de Redes

| Tipo | Descrição | Ícone |
|------|-----------|-------|
| **LAN (Local Area Network)** | Rede local, geralmente dentro de uma empresa ou casa | 🏠 |
| **WAN (Wide Area Network)** | Rede que cobre grandes áreas geográficas | 🌎 |
| **MAN (Metropolitan Area Network)** | Rede que cobre uma cidade ou campus | 🏙️ |
| **PAN (Personal Area Network)** | Rede pessoal, como Bluetooth ou cabos USB | 📱 |
| **VPN (Virtual Private Network)** | Rede privada sobre a internet pública | 🔒 |

---

## ⚙️ Componentes Principais

- **Roteadores (Routers)** – 🔀 Direcionam pacotes entre redes  
- **Switches** – 🔗 Conectam múltiplos dispositivos dentro de uma LAN  
- **Access Points (APs)** – 📡 Proporcionam conectividade sem fio  
- **Firewalls** – 🛡 Controlam acesso e protegem redes  
- **Servidores** – 🖥 Servem dados, aplicativos e serviços  

---

## 📊 Protocolos Fundamentais

| Protocolo | Camada | Função | Emoji |
|-----------|--------|--------|-------|
| **TCP/IP** | Transporte / Internet | Confiável, orientado a conexão | 🔗 |
| **UDP** | Transporte | Rápido, sem confirmação | ⚡ |
| **HTTP / HTTPS** | Aplicação | Transferência de páginas web | 🌐 |
| **FTP / SFTP** | Aplicação | Transferência de arquivos | 📁 |
| **DNS** | Aplicação | Tradução de nomes de domínio | 🧭 |
| **DHCP** | Aplicação | Distribuição automática de IPs | 🖧 |

---

## 🌐 Topologias de Rede

- 🔹 **Estrela (Star)** – Todos os dispositivos conectados a um switch central  
- 🔹 **Barramento (Bus)** – Todos compartilham um único cabo principal  
- 🔹 **Anel (Ring)** – Pacotes circulam em um anel fechado  
- 🔹 **Malha (Mesh)** – Cada dispositivo conectado a todos os outros  

---

## 💡 Boas Práticas em Redes

1. 🔹 Documentar toda a rede e IPs  
2. 🔹 Segmentar redes com VLANs para segurança  
3. 🔹 Monitorar tráfego e performance  
4. 🔹 Atualizar firmware e softwares de rede regularmente  
5. 🔹 Implementar políticas de acesso e autenticação  

---

## 🚀 Benefícios

- ⚡ Comunicação rápida e eficiente  
- 🌍 Compartilhamento de recursos e dados  
- 🛡 Segurança com segmentação e firewalls  
- 📈 Escalabilidade e flexibilidade  

---

## 🔗 Referências

- [Cisco Networking Basics](https://www.cisco.com/c/en/us/solutions/small-business/resource-center/networking.html) 🌐  
- [CompTIA Network+](https://www.comptia.org/certifications/network) 🏆  
- [OWASP Network Security Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Network_Security_Cheat_Sheet.html) 🔒  
- [Wikipedia: Computer Network](https://en.wikipedia.org/wiki/Computer_network) 📚  

---

> 🌟 Redes bem projetadas não apenas conectam computadores, mas conectam pessoas, empresas e o mundo digital com segurança e eficiência.


# 🔐 Segurança de Redes — Foco na Camada 4 (Transporte)

A camada 4 é onde o tráfego deixa de ser só “dados” e vira **conexões reais**, com portas, estados e fluxos controlados. É também o ponto onde a maioria dos ataques práticos ocorre, porque aqui vivem **TCP, UDP, multiplexação e gerenciamento de sessões** — tudo aquilo que firewalls, scanners e atacantes adoram explorar.

Este repositório centraliza estudos, anotações e testes práticos sobre segurança focada especificamente na camada de transporte.

---

## ⚙️ O que a Camada 4 governa
- Portas TCP/UDP  
- Estabelecimento e encerramento de conexões  
- Controle e confiabilidade (TCP)  
- Comunicação sem estado (UDP)  
- Multiplexação de serviços  
- Controle de fluxo e congestionamento (TCP)

Quando você deixa essa camada mal configurada, vira buffet livre para scanners, brute force, flooding e qualquer tráfego indesejado.

---

## 🚨 Principais riscos na Camada 4

### **1. Portas expostas desnecessariamente**
Cada porta aberta é uma porta de entrada.  
Ataques comuns:
- Enumeração com Nmap  
- Fingerprinting de serviços  
- Testes de brute force  
- Exploração de serviços vulneráveis

---

### **2. Ataques de flooding**
- **TCP SYN Flood**: esgota a fila de half-open connections.  
- **UDP Flood**: satura banda e CPU.  
- **RST Flood / ACK Flood**: instabilidade e perda de sessão.  

Ataques de camada 4 são baratos, difíceis de diferenciar de tráfego legítimo e eficientes contra servidores mal configurados.

---

### **3. Manipulação de flags TCP**
Atacantes usam pacotes:
- FIN  
- XMAS  
- NULL  
…para tentar burlar firewalls ruins ou mapear serviços discretamente.

---

### **4. Bypass de firewall mal configurado**
Se o firewall não entende **estado** (stateful inspection), basta o atacante:
- forjar flags  
- enviar tráfego inesperado  
- abusar de respostas abertas  
para passar.

Camada 4 é onde um firewall incompetente se entrega.

---

### **5. Amplificação via UDP**
Protocolos mal protegidos (NTP, SSDP, DNS aberto) podem gerar ataques de amplificação devastadores, explorando o fato de o UDP não ter handshake.

---

## 🧰 Defesa prática na Camada 4

### 🔒 **1. Firewalls stateful bem configurados**
Regras que levam em conta o estado da conexão, não só portas.

### 🔒 **2. Fechar tudo — abrir só o necessário**
Regra de ouro: **“deny any” → permitir caso a caso.**

### 🔒 **3. Filtragem por porta e protocolo**
Nada de deixar:
- SSH (22) exposto  
- RDP (3389) aberto  
- DBs expostos (3306, 5432, 27017)  

Se expôs, vai ser varrido.

---

### 🔒 **4. Rate limiting e mitigação de DoS**
- SYN cookies  
- Limite por IP  
- Timeouts curtos  
- Limitar half-open connections  
- Monitoramento agressivo de picos

---

### 🔒 **5. IDS/IPS focado em anomalias de transporte**
Detectar:
- flags estranhas  
- varreduras furtivas  
- assinaturas de flood  
- tráfego inconsistente entre fluxos

---

## 📡 Ferramentas importantes
- **Nmap** → análise de portas e serviços  
- **tcpdump** → captura de tráfego por porta/protocolo  
- **Wireshark** → inspeção de flags e fluxos TCP  
- **iptables/nftables** → controle fino da Camada 4  
- **fail2ban** → bloquear brute force  
- **pfSense/OPNsense** → firewall stateful robusto  


