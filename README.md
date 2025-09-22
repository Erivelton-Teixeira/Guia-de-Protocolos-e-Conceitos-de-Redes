# 🌐 Guia Completo de Protocolos e Conceitos de Redes
Este documento explica de forma simples os principais protocolos, dispositivos e conceitos de redes de computadores.


## 📜 Protocolos

### 🔹 Protocolo

Um **protocolo** é um conjunto de **regras de comunicação**. Ele define como computadores conversam entre si.

---

### 🔹 IP (Internet Protocol)

* Funciona como o **endereço da casa** de cada computador na rede.
* Sem ele, não é possível entregar pacotes.

---

### 🔹 TCP/IP

* Combinação de dois protocolos:

  * **IP** → endereço de origem e destino.
  * **TCP** → garante que os pacotes cheguem inteiros e organizados.
* 📦 É como um pacote com endereço (IP) e rastreamento (TCP).

---

### 🔹 Pacotes Novell (IPX/SPX)

* Antigo protocolo usado em redes **Novell**.
* Hoje está em desuso, substituído pelo TCP/IP.

---

### 🔹 Pacotes Apple (AppleTalk)

* Protocolo de rede usado por computadores da Apple.
* Substituído pelo TCP/IP.

---

### 🔹 ICMP (Internet Control Message Protocol)

* Usado para mensagens de **controle da rede**.
* Exemplo: comando **ping**.

---

### 🔹 Ping da Morte

* Ataque antigo que enviava pacotes **ICMP enormes**, causando travamentos.
* Hoje em dia os sistemas já bloqueiam isso.

---

## ⚙️ Componentes de Rede

### 🔹 Interface de Rede

* Dispositivo (placa ou adaptador) que conecta o computador à rede.

---

### 🔹 LAN, WAN, MAN, RAN, CAN, PAN, SAN, WLAN

* **LAN (Local Area Network)** → Rede local (ex.: dentro de uma empresa ou casa).
* **WAN (Wide Area Network)** → Rede ampla (ex.: a Internet).
* **MAN (Metropolitan Area Network)** → Rede de uma cidade.
* **RAN (Regional Area Network)** → Rede de uma região.
* **CAN (Campus Area Network)** → Rede de um campus universitário ou empresa.
* **PAN (Personal Area Network)** → Rede pessoal (Bluetooth, por exemplo).
* **SAN (Storage Area Network)** → Rede dedicada a armazenamento.
* **WLAN (Wireless LAN)** → Rede local sem fio (Wi-Fi).

---

### 🔹 Diferença entre LAN e WAN

* **LAN** → Menor alcance, maior velocidade, hardware mais barato (Switches, cabos Ethernet).
* **WAN** → Maior alcance, menor velocidade em comparação, hardware mais caro (roteadores, links dedicados).

---

### 🔹 Colisão (CSMA/CD)

* Em redes antigas com **HUBs**, dois computadores podiam transmitir ao mesmo tempo → colisão.
* O protocolo **CSMA/CD** cuidava de organizar essas transmissões.
* Hoje, com **Switches**, quase não há colisões.

---

### 🔹 HUB

* Dispositivo simples que **repete** os sinais para todas as portas.
* Causa colisões porque envia dados para todos.

---

### 🔹 Switch

* Dispositivo que **envia os dados apenas para o destino correto**.
* Evita colisões e é muito mais eficiente que o HUB.

---

### 🔹 Router (Roteador)

* Dispositivo que conecta redes diferentes.
* Decide o **melhor caminho** para os pacotes.

**Quando o Router não conhece o caminho:**

* Ele envia para o **gateway padrão** ou responde com um erro ICMP ("destino inacessível").

---

### 🔹 Quando um Pacote não chega até o destino

* O remetente não recebe a confirmação do TCP.
* O TCP então reenvia o pacote.
* Se mesmo assim não chegar, ocorre erro de comunicação.

---

## 🔄 Protocolos de Transporte

### 🔹 TCP (Transmission Control Protocol)

* Confiável.
* Garante a entrega dos pacotes, verifica ordem e integridade.
* Usado em: web (HTTP/HTTPS), e-mail, etc.

### 🔹 UDP (User Datagram Protocol)

* Mais rápido, mas **não confiável**.
* Não confirma entrega.
* Usado em: jogos online, chamadas de vídeo, streaming.

---

## 🔐 Segurança e Controle

### 🔹 Proxy

* Servidor que **intermedia** o acesso entre usuário e internet.

**Funções do Proxy:**

* Armazenar páginas em cache (mais rápido).
* Filtrar acessos (bloquear sites).
* Aumentar a segurança.

---

### 🔹 Firewall

* Sistema que **controla o tráfego de rede**.
* Decide o que pode ou não passar (como um porteiro).

---

### 🔹 Portas

* Cada serviço usa uma **porta** para se comunicar.
* Exemplo: uma casa com várias portas de entrada, cada uma para um serviço.

**Principais portas:**

* **80** → HTTP (páginas web).
* **110** → POP3 (receber e-mails).
* **25** → SMTP (enviar e-mails).
* **21** → FTP (transferência de arquivos).
* **23** → Telnet (acesso remoto antigo).

---

### 🔹 DNS (Domain Name System)

* Sistema que traduz **nomes de sites** (ex.: [www.google.com](http://www.google.com)) em **endereços IP**.
* Funciona como uma lista telefônica da internet.

---

## 📌 Resumo Final

* **Protocolo** → Regras de comunicação.
* **IP** → Endereço.
* **TCP** → Confiável, garante entrega.
* **UDP** → Rápido, mas sem garantia.
* **ICMP** → Testa conexões (ping).
* **Proxy/Firewall** → Segurança e controle.
* **Portas** → Portas de entrada de serviços.
* **LAN, WAN, etc.** → Tipos de redes.
* **Switch/Router/HUB** → Dispositivos de rede.
* **DNS** → Tradutor de nomes para IPs.

