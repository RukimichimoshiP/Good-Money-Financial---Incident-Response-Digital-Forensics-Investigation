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

*(Adicione aqui as melhores capturas de tela)*

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

---

**Quer que eu gere agora:**

1. O README.md completo e bonito?
2. Uma versão resumida para LinkedIn (post + descrição do projeto)?
3. Sugestões de melhorias no seu relatório atual (erros, formatação, etc.)?
4. Um template de "Case Study" ainda mais profissional?

Me diga qual caminho você quer seguir primeiro e eu gero o conteúdo pronto para você copiar. 

Esse projeto tem potencial para ficar **muito forte** no seu portfólio!
