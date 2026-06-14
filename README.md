# Good-Money-Financial---Incident-Response-Digital-Forensics-Investigation

**Análise completa de um incidente de Macro Malware + Investigação Forense em imagem de disco.**

<img width="1024" height="506" alt="image" src="https://github.com/user-attachments/assets/50d9fb75-78a2-4885-89c2-be909ed54dc0" />

## 🎯 Objetivo do Projeto

Realizar a **Resposta a Incidentes** e **Análise Forense** completa de um caso realístico envolvendo:
- Análise de tráfego de rede (PCAP)
- Detecção de Macro Malware
- Investigação forense em imagem de disco Windows XP

## 🛠️ Ferramentas Utilizadas

- **Zeek (Bro)** → Análise de PCAP e geração de logs
- **Zeek-cut** → Extração e filtragem de dados
- **Autopsy** → Análise forense da imagem de disco
- **Registry Analysis, Timeline, File Carving**

## 📋 Principais Descobertas

- Identificação do host comprometido: **Nalyvaiko-PC** (172.17.1.129)
- MAC Address: `00:1e:67:4a:d7:5c`
- Vetor inicial: Documento Word malicioso (`2018_11Details_zur_Transaktion.doc`)
- Tipo de infecção: **Macro Malware**
- Download de payload: `6169583.exe`
- Ferramentas maliciosas encontradas no disco: Cain & Abel, Network Stumbler, Ethereal, WinPcap, etc.
- Último usuário: **Mr. Evil**

## 🧩 Metodologia

### Parte 1 - Incident Response (Network Forensics)
- Processamento do PCAP com Zeek
- Análise dos logs (`dhcp.log`, `http.log`, `files.log`)
- Identificação de IoCs (IPs, URLs, arquivos)

### Parte 2 - Digital Forensics
- Verificação de integridade da imagem (`MD5`)
- Análise do Registry (SYSTEM, SOFTWARE, SAM)
- Construção de Timeline de eventos
- Análise de programas instalados e Lixeira

## 📊 Relatório Completo

[Baixar Relatório Completo (PDF)](Relatorio_Completo.pdf)

## 🖼️ Screenshots

<img width="1872" height="958" alt="Atividade 1 e 2" src="https://github.com/user-attachments/assets/e94ca45b-493f-4253-93a6-bdb519bdb230" />
<img width="1780" height="958" alt="Atividade 3" src="https://github.com/user-attachments/assets/b5b27ee1-e3d8-49bb-977c-5f2319268a38" />
<img width="1780" height="958" alt="Atividade 4" src="https://github.com/user-attachments/assets/82b1350b-6778-4414-b932-38553b954a09" />

<img width="1872" height="958" alt="Questão 4" src="https://github.com/user-attachments/assets/762aaad3-c640-4d78-a45b-147ece62c834" />
<img width="1920" height="1036" alt="Pasted image 20260613154443" src="https://github.com/user-attachments/assets/19e9e94e-b505-433a-bec1-0837a6f74bb9" />
<img width="1804" height="958" alt="Questão 2 B" src="https://github.com/user-attachments/assets/c2349afa-28ce-41bf-a7f7-3a1eb4782af9" />


## 💡 Aprendizados e Lições

- Importância da segmentação de rede e bloqueio de macros
- Valor da análise comportamental em incidentes
- Correlação entre Network Forensics e Host Forensics

## 🚀 Habilidades Demonstradas

- Incident Response
- Network Forensics (Zeek)
- Digital Forensics (Autopsy)
- Análise de Malware
- Elaboração de relatórios técnicos e Laudos Periciais
- CTI (Cyber Threat Intelligence)
