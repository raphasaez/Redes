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
# 🧵 Camada 1 – Física

A Camada 1 do modelo OSI é onde tudo começa. É a base bruta da comunicação: sinais elétricos, ópticos e radiofrequência. Se essa camada falha, o resto da rede nem chega a existir. Em ambientes corporativos, ela é crítica porque define **confiabilidade**, **desempenho** e **limites físicos** da infraestrutura.

---

## 🔌 O que a Camada 1 realmente trata

- Cabos, conectores e padrões físicos  
- Sinalização (eletrônica, óptica, RF)  
- Topologias físicas  
- Especificações mecânicas e elétricas  
- Meios de transmissão  
- Limites de distância e interferência  

Sem protocolos, sem endereços, sem lógica. Só bits crus se movendo.

---

## 🧱 Principais meios físicos em redes corporativas

### **1. Par trançado (Ethernet cobre)**
- Cat5e, Cat6, Cat6A, Cat7  
- Limite típico: 100 m  
- Suporta até 10Gbps (em Cat6A)  
- Sensível a interferência eletromagnética  
- Mais comum em redes LAN corporativas  

### **2. Fibra óptica**
- Single-mode (longa distância, backbone)  
- Multi-mode (curta distância, datacenters)  
- Imune a EMI  
- Suporta dezenas de quilômetros  
- Usada para uplinks de alta capacidade  

### **3. Rádio/Wireless**
- Wi-Fi corporativo (2.4GHz / 5GHz / 6GHz)  
- Antenas direcionais para links P2P  
- Propenso a interferências e atenuação  

---

## 🔧 Componentes de Camada 1

### **Patch panels**
Organizam terminação de cabos.

### **Racks e bandejamento**
Infraestrutura física para organização.

### **Modems, amplificadores, repetidores**
Esticam alcance e regeneram sinais.

### **Transceivers (SFP, SFP+, QSFP)**
Conversão óptico/elétrico.

---

## 📡 Sinalização e características elétricas

- Codificação de linha (NRZ, PAM-4 etc.)  
- Atenuação  
- Crosstalk  
- Impedância e blindagem  
- Taxas de erro (BER)

Esses fatores determinam a estabilidade de links críticos, como servidores, switches core e storages.

---

## 🏗️ Boas práticas para redes corporativas

- Seguir normas TIA/EIA-568  
- Evitar curvar cabos acima do limite  
- Manter separação entre cabos elétricos e de dados  
- Usar fibra no backbone  
- Testar cabos com certificadores profissionais (Fluke)  
- Racks organizados → menos perda de tempo na manutenção  

---

## 🔥 Riscos comuns na Camada 1

- Cabos mal crimpados  
- Cabos baratos fora de padrão  
- Interferência de motores, UPS, iluminação industrial  
- Fibra suja ou mal polida  
- Patch cords ruins conectados a infraestrutura boa  

---

## 🛠️ Troubleshooting básico

- Teste de continuidade  
- Certificação de cabo  
- Loopback  
- Troca de patch cord  
- Verificação de porta física (LEDs)  
- Ajustar autonegociação (caso extremo)  

---

## 🎯 Por que a Camada 1 importa?

Porque você pode ter VLAN, firewall, IDS, roteamento avançado…  
Mas **se o bit não chegar inteiro**, o resto é irrelevante.

> 🌟 Redes bem projetadas não apenas conectam computadores, mas conectam pessoas, empresas e o mundo digital com segurança e eficiência.

---

# 🔗 Camada 2 – Enlace de Dados

A Camada 2 do modelo OSI controla como os dispositivos compartilham o meio físico e garante que os quadros (frames) trafeguem com integridade dentro de uma mesma rede local. É a camada que realmente dá “forma” à LAN corporativa.

---

## 🧩 O que a Camada 2 trata

- Endereçamento MAC  
- Switches e bridges  
- Detecção e prevenção de colisões  
- VLANs  
- Trunking (802.1Q)  
- STP e suas variantes  
- Controle de fluxo  
- QoS básica (priorização L2)  

A Camada 2 define como os quadros se movem entre hosts **sem depender de roteamento**.

---

## 🧬 Endereçamento MAC

Cada interface de rede possui um endereço físico único.  
A Camada 2 depende deste endereço para entregar frames dentro da mesma LAN.

- 48 bits  
- Hexadecimal  
- Formato: `AA:BB:CC:DD:EE:FF`

---

## 🔀 Switches (O cérebro da LAN)

### O que eles fazem:
- Aprendem MACs dinamicamente  
- Fazem forwarding inteligente (não broadcast)  
- Suportam segmentação lógica via VLAN  
- Evitam loops com STP  
- Garantem full-duplex e redução de colisões  

São o coração da infraestrutura interna corporativa.

---

## 🧱 VLANs (Virtual LANs)

VLANs segmentam a rede lógica sem alterar o cabeamento físico.

### Benefícios:
- Maior segurança interna  
- Menos broadcast  
- Segmentação por setores  
- Isolamento de servidores críticos  
- Facilita políticas de acesso  

### Tipos:
- **Access**: porta pertence a uma VLAN fixa  
- **Trunk**: carrega múltiplas VLANs usando uma tag 802.1Q  

---

## 🌉 STP – Spanning Tree Protocol

Evita loops em topologias corporativas com redundância.

### Variantes:
- STP  
- RSTP  
- MSTP  

### Problemas comuns:
- Convergência lenta (em STP clássico)  
- Porta em estado errado  
- Configurações erradas de prioridade  

---

## 📶 Controle de fluxo e QoS L2

- Pause frames (802.3x)  
- Priorização L2 (CoS – 802.1p)  
- Redução de congestionamento em links internos  

Especialmente útil em ambientes com VoIP, câmeras e serviços sensíveis a latência.

---

## 📡 Protocolos e tecnologias relevantes

- **Ethernet** (o padrão dominante)  
- **LLDP** (descoberta de vizinhança)  
- **LACP** (agregação de links – 802.3ad)  
- **ARP** (técnico na L2.5, mas impacta diretamente a LAN)  
- **CDP** (Cisco Discovery Protocol)  

---

## 🛡️ Segurança em Camada 2

A camada 2 é um alvo direto em redes corporativas. É aqui que ocorrem ataques “silenciosos”.

### Principais riscos:
- ARP Spoofing / ARP Poisoning  
- MAC Flooding  
- Port Stealing  
- VLAN Hopping  
- STP Manipulation  
- Rogue Switches  

### Contramedidas:
- Port Security  
- Dynamic ARP Inspection  
- DHCP Snooping  
- BPDU Guard  
- Root Guard  
- Storm Control  

---

## 🛠️ Troubleshooting na prática

- Verificar tabela MAC do switch  
- Checar VLAN da porta  
- Conferir trunks e tags  
- Analise de BPDUs  
- Loop detection  
- Monitoramento de broadcast/multicast  

Switch configurado errado = metade da empresa parada.

---

## 🎯 Por que a Camada 2 importa?

Porque é nela que a LAN vive.  
É nela que você controla quem fala com quem, como os quadros trafegam e como você mantém a rede interna segura e organizada.

Sem uma Camada 2 sólida, qualquer iniciativa de segurança ou roteamento vira caos.

---

# 🌐 Camada 3 – Rede

A Camada 3 do modelo OSI é responsável pelo **endereçamento lógico**, **roteamento** e **comunicação entre redes distintas**.  
É aqui que a LAN deixa de ser um ambiente isolado e passa a conversar com outras sub-redes, filiais, datacenters e a internet.

---

## 🧠 O que a Camada 3 controla

- Endereçamento IP  
- Sub-redes e máscaras  
- Roteamento (estático e dinâmico)  
- Gateways  
- Fragmentação de pacotes  
- Tráfego entre VLANs (Inter-VLAN Routing)  
- Filtragem básica por ACLs  
- Protocolos de descoberta e resolução (ICMP / ARP)  

Se a Camada 2 organiza a LAN, **a Camada 3 decide para onde os pacotes vão**.

---

## 🧭 Endereçamento IP

A base da comunicação L3 é o endereço IP.

### IPv4:
- 32 bits  
- 4.3 bilhões de endereços (já exaustos)  
- Utiliza NAT para suportar escala  

### IPv6:
- 128 bits  
- Espaço virtualmente inesgotável  
- Segurança nativa (IPsec integrado)  

### Máscara de sub-rede
Define:
- Tamanho da sub-rede  
- Quantidade de hosts  
- Limites de broadcast  

Exemplo:  
`192.168.10.0/24` → 254 hosts possíveis.

---

## 🚦 Roteadores

Roteadores são o núcleo da Camada 3.

### Funções essenciais:
- Tomada de decisão por IP  
- Interconexão entre redes  
- Inter-VLAN routing  
- Segmentação lógica avançada  
- Aplicação de ACLs (filtro L3/L4)  
- Encapsulamento de tráfego para WAN/VPN  
- Comunicação com switches via interfaces trunk ou routed  

Sem roteador, a empresa fica presa em uma única LAN gigante e insegura.

---

## 🔀 Roteamento

### ✔️ Roteamento Estático
- Totalmente manual  
- Usado para redes pequenas e rotas simples  
- Previsível, porém rígido  

### ✔️ Roteamento Dinâmico
Utiliza protocolos para trocar rotas automaticamente.

Principais:
- **OSPF** (intraempresa, roteamento interno)  
- **EIGRP** (Cisco)  
- **BGP** (WAN e internet, provedores)  

Benefícios:
- Convergência automática  
- Redundância  
- Balanceamento de carga  

Em ambientes corporativos médios e grandes, **OSPF** domina.

---

## 🔄 NAT — Network Address Translation
O **NAT** permite que vários dispositivos da rede interna acessem a internet usando **um único endereço IPv4 público**.  
Sem ele, o esgotamento de IPv4 tornaria muitas redes inviáveis.

**Funções principais:**
- Ocultar IPs internos (segurança básica).
- Economizar endereços públicos.
- Permitir comunicação entre redes com espaçamentos privados.

**Tipos mais comuns:**
- **SNAT** — Source NAT (alteração do IP de origem).
- **DNAT** — Destination NAT (redirecionamento de portas).
- **PAT** — Port Address Translation (o mais comum, usado em roteadores domésticos).

---

## 🧩 DHCP — Dynamic Host Configuration Protocol
O **DHCP** automatiza a entrega de configurações IP para as máquinas da rede.  
Dispensa configuração manual e evita conflitos.

**Entrega automaticamente:**
- Endereço **IP**
- **Máscara** de rede
- **Gateway** padrão
- **DNS**
- Tempo de concessão (**lease time**)

**Benefícios:**
- Reduz erros humanos  
- Torna a gestão da rede mais simples  
- Muito usado em redes corporativas e domésticas  

---

## 🚪 Gateway — Porta de Saída da Rede
O **gateway padrão** é o equipamento que **interliga sua LAN ao resto do mundo**.  
É, basicamente, o dispositivo que recebe pacotes destinados a outras redes.

**Exemplos de gateway:**
- Roteador corporativo
- Firewall
- Switch Layer 3
- Equipamento de borda do provedor

**Função essencial:**
> Sem um gateway, os hosts só conversam dentro da própria LAN.

---

## 📌 Relação entre eles
- O **gateway** é quem normalmente implementa **NAT** para acessar a internet.  
- O **DHCP** entrega automaticamente o **gateway padrão** aos dispositivos.  
- Juntos, mantêm a rede funcional, escalável e administrável.

## 🛠️ ARP – Address Resolution Protocol

ARP é L2.5, mas essencial na Camada 3.  
Ele traduz **IP → MAC** para permitir que pacotes IP sejam entregues via Ethernet.

Sem ARP:
- Nada na LAN funciona  
- Clientes não alcançam o gateway  
- Roteadores não comunicam com switches  

Também é alvo comum de ataques internos (ARP Spoofing).

---

## 📡 Access Points na Camada 3

Access Points corporativos vão muito além de “wifi”.

Funções L3:
- Atribuição de VLAN por SSID  
- Autenticação 802.1X (via Radius)  
- DHCP relay  
- Captive Portal  
- Controle via CAPWAP (gerenciamento centralizado)  
- Firewall básico em alguns modelos  
- Roteamento local em APs com NAT (dependendo da arquitetura)  

AP bem configurado = Wi-Fi estável, isolado e seguro.

---

## 🔐 Segurança em Camada 3

A Camada 3 é onde as políticas realmente começam a ganhar força.

### Controles típicos:
- ACLs (permit/deny baseado em IP e portas)  
- Segmentação por sub-redes  
- Isolamento entre departamentos via inter-VLAN  
- Filtragem de ICMP  
- Controle de tráfego lateral  
- Firewalls de borda  

### Riscos comuns:
- Máscaras erradas  
- Gateways duplicados  
- Roteamento sobreposto  
- Falhas em ACLs expondo servidores  
- ARP poisoning afetando roteamento local  

---

## 📈 Troubleshooting L3 na prática

- `ping` (testar reachabilidade)  
- `traceroute`  
- Verificação de gateway padrão  
- Conferência de rotas (`ip route`, `show ip route`)  
- Checagem de ARP (`arp -a`, `show ip arp`)  
- Análise de ICMP  
- Loopback tests  

90% dos problemas corporativos de rede são erros de gateway, rota ou máscara.

---

## 🎯 Por que a Camada 3 importa?

Porque é ela que **faz a empresa funcionar como várias redes bem organizadas**, e não como um amontoado de máquinas brigando por broadcast.

Sem Camada 3 configurada direito:
- Wi-Fi falha  
- Filiais não se conectam  
- Servidores ficam inacessíveis  
- Firewalls perdem eficácia  
- A LAN vira um caos de broadcast  

A Camada 3 é o ponto onde **rede, segurança e arquitetura se unem**.

---
# 🚚 Camada 4 — Transporte
A Camada 4 é responsável por garantir **como** os dados trafegam entre origem e destino — confiável, rápido ou simples.  
Ela lida com **conexões**, **controle de fluxo**, **portas** e **segmentação**.

---

## 🔢 Portas — A Identidade dos Serviços
Portas definem **qual aplicação** deve receber o tráfego.

- **0–1023** → Portas bem conhecidas (HTTP 80, HTTPS 443, DNS 53, SSH 22)  
- **1024–49151** → Portas registradas  
- **49152–65535** → Portas dinâmicas / efêmeras

**Por que isso importa em redes corporativas?**  
Firewalls, NACLs, proxies e IDS dependem de portas para criar regras de segurança.

---

## 🔄 TCP — Conexão Confiável
TCP oferece **entrega garantida**, ordenada e com controle de fluxo.

### Características:
- Conexão orientada (**3-way handshake**)  
- Retransmissão de pacotes perdidos  
- Janela deslizante (flow control)  
- Congestion control  

### Usado em:
- HTTP/HTTPS  
- SSH  
- FTP  
- E-mail (IMAP, SMTP com TLS)  

**Vantagem:** confiabilidade  
**Desvantagem:** overhead maior

---

## ⚡ UDP — Velocidade sem Frescura
UDP é **não confiável**, mas extremamente rápido.

### Características:
- Sem handshake  
- Sem retransmissão  
- Baixa latência  

### Usado em:
- DNS  
- VoIP  
- Jogos online  
- Streaming  
- Broadcast/multicast  

**Vantagem:** velocidade  
**Desvantagem:** sem garantia de entrega

---

## 🧱 Firewalls e a Camada 4
Grande parte dos firewalls trabalha **no mínimo até a camada 4**, analisando:
- Porta  
- Protocolo (TCP/UDP)  
- Estado da conexão (stateful firewall)  
- Flags TCP (SYN, ACK, FIN, RST)  

A camada 4 é onde surge o conceito de:
- **Allow/Deny baseado em portas**
- **Stateful inspection**
- **Port knocking**
- **TCP/UDP filtering**

---

## 📦 Segmentação e Reassembly
A Camada 4 divide dados em:
- **Segs. TCP**
- **Datagramas UDP**

Ela gerencia:
- Tamanho dos segmentos (**MSS**)  
- Velocidade (**flow control**)  
- Detecção de perda (**retransmission**)  

---

## 🕵 Monitoramento e Segurança
Ferramentas essenciais focadas na Camada 4:

- **Nmap** (SYN scan, ACK scan, UDP scan)  
- **Netstat / ss**  
- **TCPDump / Wireshark**  
- **Hping3** (crafting de pacotes)  

A camada 4 revela:
- Serviços expostos  
- Portas vulneráveis  
- Tentativas de conexão indevidas  
- Tráfego suspeito em protocolos críticos  

---

## 🧠 Resumo Direto
- **TCP = confiabilidade**  
- **UDP = velocidade**  
- **Portas determinam a aplicação-alvo**  
- **Firewalls dependem fortemente da camada 4**  
- **Monitoramento e pentest focam muito aqui**  

A Camada 4 é onde a rede deixa de ser apenas “tráfego” e passa a ser **comunicação real entre aplicações**.

===

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

---

# 🛡️ Camada 7 — Aplicação  
Segurança na Camada mais Crítica da Rede

A Camada 7 é onde tudo realmente acontece: APIs, web apps, autenticação, bancos de dados, sistemas corporativos, SaaS…  
E, por isso, **é a camada mais atacada e explorada da segurança moderna**.

---

# 🎯 Por que a Camada 7 é crítica?
Enquanto as camadas 1–4 lidam com transporte, velocidade, roteamento e portas…  
A Camada 7 lida com **lógica de aplicação**, onde o atacante pode manipular:

- Requisições HTTP/HTTPS  
- Parâmetros, headers, cookies  
- Sessões e tokens  
- Serialização  
- Uploads  
- APIs REST/GraphQL  
- Autenticação e autorização  

Quando essa camada falha, a rede inteira cai junto.

---

# 🔥 Principais Ameaças da Camada 7

## 1. **OWASP Top 10**
A lista mais relevante do mundo para segurança de aplicações.

Inclui ameaças como:
- Injeções (SQLi, NoSQLi, LDAPi)  
- Quebra de autenticação  
- Exposição de dados sensíveis  
- Falhas de autorização  
- SSRF  
- RCE  
- Deserialização insegura  
- Controle inadequado de acesso  

Essas falhas são responsáveis pela maior parte dos incidentes reais.

---

## 2. **Ataques Contra APIs**
APIs são hoje o principal alvo corporativo.

Riscos comuns:
- Bypass de autenticação  
- Rate limit inexistente  
- Exposição de dados internos  
- API Keys vazadas  
- Inadequate Authorization (IDOR)  
- GraphQL introspection aberta  

APIs mal configuradas servem de pivô para ataques maiores.

---

## 3. **Manipulação de Sessão**
Tudo relacionado a login e persistência do usuário é crítico.

Riscos:
- Cookies sem `HttpOnly` e `Secure`  
- Sessões previsíveis  
- JWT sem expiração  
- Reuso de tokens  
- Falta de rotação após login  

Um erro aqui e o atacante se torna o usuário.

---

## 4. **Ataques HTTP Exploratórios**
A Camada 7 permite ataques complexos e difíceis de detectar:

- Slowloris  
- HTTP Request Smuggling  
- HTTP Response Splitting  
- Header Injection  
- Cache Poisoning  
- Host Header Attack  

Esse tipo de ataque **contorna firewalls tradicionais**.

---

## 5. **Upload e Manipulação de Arquivos**
Um dos vetores mais perigosos.

Falhas comuns:
- Upload de webshell  
- Validação fraca de extensão/MIME  
- Upload de `.php`, `.jsp`, `.aspx` disfarçado  
- Path traversal  
- Exploitação de imagem/PDF (XXE, payloads)  

Aplicação sem validação de upload é suicídio.

---

# 🧱 Controles de Defesa para Camada 7

## 🔐 1. Autenticação e Autorização Fortes
- MFA obrigatório  
- Tokens com expiração curta  
- Sessão rotacionada após login  
- Políticas de RBAC/ABAC  

---

## 📊 2. Monitoramento e Observabilidade
- WAF com regras atualizadas  
- IDS/IPS com inspeção profunda (DPI)  
- Rate limit e throttling  
- Logging detalhado com correlação  
- Análise de User-Agent, IP, ASN  

Não dá para proteger o que você não vê.

---

## 🛡️ 3. WAF (Web Application Firewall)
WAF moderno filtra tráfego malicioso em:

- SQLi  
- XSS  
- LFI/RFI  
- Force brute  
- Exploits automatizados  
- Ataques de bots  

Ferramentas:  
Cloudflare WAF • ModSecurity • AWS WAF • F5 ASM

---

## 🔧 4. Hardening e Boas Práticas
- Desabilitar portas e endpoints desnecessários  
- Sanitização de input e output  
- Headers de segurança:  
  - `X-Frame-Options`  
  - `Content-Security-Policy`  
  - `Strict-Transport-Security`  
  - `X-Content-Type-Options`  
- TLS forçado  
- Taxas máximas por IP  

---

## 🚨 5. Proteção de API
- Rate limit por chave  
- Rotação de tokens  
- Escopo de permissões  
- Filtering de IP/origem  
- Validação rígida do schema  
- Remover debug e introspection  

---

# 🧪 Ferramentas para Pentest em Camada 7

- **Burp Suite / OWASP ZAP** (principal)  
- **Nmap NSE scripts**  
- **Nikto**  
- **sqlmap**  
- **Feroxbuster / Gobuster**  
- **ffuf**  
- **WFuzz**  
- **Postman / Insomnia**  
- **httpx / nuclei**  

---

# 🧩 Resumo Final
A Camada 7 é onde estão:
- As aplicações  
- Os usuários  
- Os dados  
- Os serviços críticos  
- As APIs  
- Os ataques mais sofisticados  

É também onde ocorre **90% das invasões modernas**.

Ignorar segurança na Camada 7 é ignorar o ponto mais vulnerável da empresa.

---

# 📢 Quer se aprofundar nas vulnerabilidades da Camada 7?

Se você chegou até aqui, vale dar um passo além.  
Preparei um repositório **dedicado ao OWASP Top 10**, onde destrincho cada vulnerabilidade com:

- Exemplos práticos  
- Explicações técnicas  
- Cenários reais  
- Vetores de ataque  
- Formas de mitigação  
- Demonstrações e payloads  

Se a Camada 7 é o ponto mais atacado da segurança moderna, o **OWASP 10 é o mapa do campo de batalha**.
