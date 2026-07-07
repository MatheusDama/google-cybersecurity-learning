# 🛡️ Guia de Cybersecurity Tools & Concepts

Este repositório reúne um resumo prático das principais ferramentas, termos técnicos e conceitos de segurança da informação utilizados por analistas de segurança (SOC) no dia a dia para monitoramento, detecção, análise de tráfego e resposta a incidentes.

---

## 📋 Core Concepts (Conceitos Chave)

### 🪵 Log
A record of events that occur within an organization's systems and networks.
* **Por que importa:** Logs são a base da visibilidade em segurança. *They help security professionals identify vulnerabilities, track user activity, and detect potential security breaches.* Sem logs, uma organização está operando no escuro.

### 📘 Playbook
A standardized manual that provides step-by-step details about operational actions.
* **Por que importa:** Funciona como um guia de reação rápida e padronizada. *It defines exactly how to respond to specific security incidents (e.g., a phishing attack or unauthorized access), minimizing human error during a crisis.*

### 🌐 Network Protocol Analyzer (Packet Sniffer)
A tool designed to capture and analyze live data traffic traveling within a network.
* **Por que importa:** Permite inspecionar o tráfego de rede a fundo (até a camada de pacotes). *It allows analysts to dissect malicious traffic, identify unauthorized data exfiltration, or troubleshoot connectivity issues.*
* **Ferramenta Principal:** **Wireshark** (indispensável para análise de arquivos `.pcap`).

---

## 🛠️ SIEM (Security Information and Event Management)

A **SIEM** (pronounced *'sim'*) tool is an application that collects, aggregates, and analyzes log data from various sources across an organization to monitor critical activities.

> 💡 **Key Value:** SIEM tools allow security analysts to identify potential breaches and insider threats **in real-time** (as they happen), turning raw log data into actionable security intelligence through **correlation rules** (regras que ligam múltiplos eventos isolados a um ataque real).

### Plataformas de SIEM em Destaque

| Tool | Type | Key Characteristics |
| :--- | :--- | :--- |
| **Splunk Enterprise** | Self-Hosted / Hybrid | A powerful data analysis platform used to retain, analyze, and search massive amounts of an organization's log data. Uses **SPL** (Splunk Search Processing Language). |
| **Google Chronicle** | Cloud-Native | A cloud-native SIEM built on Google infrastructure, allowing for massive scaling, fast search capabilities, and rapid delivery of new features using **YARA-L** for detection rules. |
| **Microsoft Sentinel** | Cloud-Native | A scalable, cloud-native SIEM/SOAR that provides intelligent security analytics across the entire enterprise, deeply integrated with Azure ecosystem. |

---

## 🛡️ Defesa de Endpoint e Rede (Complementos Essenciais)

Para que um SIEM funcione perfeitamente, ele precisa receber dados de outras ferramentas críticas de proteção e detecção. As principais são:

### 🖥️ EDR (Endpoint Detection and Response)
Softwares avançados instalados diretamente nos dispositivos (computadores, servidores) que monitoram comportamentos suspeitos em tempo real, permitindo isolar a máquina da rede se um malware for detectado.
* *Exemplos:* CrowdStrike Falcon, Microsoft Defender for Endpoint, SentinelOne.

### 🛑 IDS / IPS (Intrusion Detection/Prevention Systems)
Sistemas posicionados na rede para inspecionar o tráfego em busca de assinaturas de ataques conhecidos ou anomalias.
* **IDS (Detecção):** Apenas monitora e gera um alerta no SIEM.
* **IPS (Prevenção):** Toma uma atitude ativa e bloqueia o tráfego malicioso imediatamente.
* *Exemplos:* Snort, Suricata.

---

## 🔍 Telemetria & Tipos de Logs Importantes

Como analista, você passará muito tempo investigando logs específicos dentro do SIEM. Estes são os mais comuns que você deve conhecer:

* **Authentication Logs (Logs de Autenticação):** Registram tentativas de login (sucessos e falhas). Essenciais para detectar ataques de *Brute Force* (Força Bruta) ou *Credential Stuffing*.
* **Firewall Logs:** Registram conexões permitidas ou bloqueadas na borda da rede. Ajudam a identificar varreduras de portas (*Port Scanning*) ou conexões com servidores maliciosos (C2 - *Command and Control*).
* **DNS Logs:** Registram quais domínios e sites os computadores internos estão tentando acessar. Cruciais para identificar se um malware está tentando se comunicar externamente ou se um usuário clicou em um link de *Phishing*.

---

## 📝 Footnotes / References

[^1]: **Telemetry (Telemetria):** A coleta e transmissão automática de dados de fontes remotas (como servidores e firewalls) para um local centralizado (como o SIEM) para fins de monitoramento e análise.
[^2]: **SOAR (Security Orchestration, Automation, and Response):** Tecnologias que complementam o SIEM, permitindo automatizar a resposta aos alertas (ex: bloquear automaticamente um IP malicioso no firewall sem intervenção humana).
[^3]: **Packet Capture (PCAP):** O formato de arquivo padrão usado para salvar dados de tráfego de rede capturados por um analisador de protocolos (como o Wireshark).
