
# 📚 CISSP Domains Overview (Guia de Consulta)

O **CISSP** (*Certified Information Systems Security Professional*) da ISC² é estruturado em **8 grandes domínios**. Eles cobrem desde a governança estratégica até a segurança física e operacional, servindo como a base conceitual para qualquer analista de segurança.

---

## 🏛️ 1. Security and Risk Management (Segurança e Gestão de Riscos)
*O "guarda-chuva" estratégico da segurança. Define as regras do jogo antes da técnica entrar em ação.*

*   **Conceitos-Chave:** A Tríade CIA (Confidencialidade, Integridade, Disponibilidade), princípios de governança de segurança, conformidade regulatória (GDPR, LGPD, PCI-DSS), ética profissional (Código de Ética ISC²), políticas de segurança e continuidade de negócios (BCP).
*   **Foco Prático:** Como quantificar o risco (ALE, SLE, ARO) e decidir se a organização vai mitigar, transferir, aceitar ou evitar o risco.

---

## 📦 2. Asset Security (Segurança de Ativos)
*Focado na proteção, classificação e ciclo de vida dos dados e recursos físicos ou digitais.*

*   **Conceitos-Chave:** Classificação de dados (público, confidencial, secreto), papéis de responsabilidade (*Data Owners* vs. *Data Custodians*), privacidade e proteção de PII/SPII, ciclo de retenção de dados e destruição segura de mídias.
*   **Foco Prático:** Garantir que os ativos da empresa sejam devidamente inventariados e recebam o nível de proteção proporcional ao seu valor e ao impacto de sua perda.

---

## 🏗️ 3. Security Architecture and Engineering (Arquitetura e Engenharia de Segurança)
*A engenharia por trás dos sistemas. Como projetar defesas robustas usando criptografia e modelos de segurança.*

*   **Conceitos-Chave:** Modelos de segurança (Bell-LaPadula, Biba), criptografia (Simétrica, Assimétrica, Hashing), segurança baseada em nuvem, vulnerabilidades de sistemas embarcados/IoT, e conceitos de design seguro (*Zero Trust*, defesa em profundidade).
*   **Foco Prático:** Implementar proteções no nível de hardware e software para que o sistema resista a falhas e ataques por design (*Security by Design*).

---

## 🌐 4. Communication and Network Security (Segurança de Redes e Comunicação)
*Como proteger os canais de transmissão e a infraestrutura física/lógica que conecta os sistemas.*

*   **Conceitos-Chave:** Arquitetura de rede segura (Modelos OSI e TCP/IP), protocolos seguros (HTTPS, SSH, IPsec), segmentação de rede (VLANs), SDN (*Software-Defined Networking*), Wi-Fi seguro e defesas contra ataques de rede (DDoS, Spoofing).
*   **Foco Prático:** Garantir que os dados em trânsito não sejam interceptados (confidencialidade) ou modificados no caminho (integridade).

---

## 🔑 5. Identity and Access Management - IAM (Gestão de Identidade e Acesso)
*Garantir que a pessoa certa (ou sistema certo) acesse o recurso certo pelas razões certas.*

*   **Conceitos-Chave:** Controle de acesso baseado em função (RBAC), ciclo de vida da identidade (provisionamento, manutenção, revogação), autenticação multifator (MFA), Federação de Identidade (SSO, SAML, OAuth) e prevenção de ataques de identidade.
*   **Foco Prático:** Aplicar estritamente o princípio do privilégio mínimo (*Least Privilege*) e a necessidade de conhecer (*Need-to-Know*).

---

## 🧪 6. Security Assessment and Testing (Avaliação e Testes de Segurança)
*Como a organização valida e testa continuamente se suas defesas realmente funcionam.*

*   **Conceitos-Chave:** Testes de invasão (*Penetration Testing*), varreduras de vulnerabilidade (*Vulnerability Scanning*), auditorias de segurança internas e externas, análise de logs e testes de software (estático/SAST e dinâmico/DAST).
*   **Foco Prático:** Encontrar as vulnerabilidades e brechas antes que um atacante (*Threat Actor*) as descubra e explore.

---

## ⚙️ 7. Security Operations (Operações de Segurança)
*O dia a dia do SOC (Security Operations Center). Onde os analistas passam a maior parte do tempo investigando e respondendo.*

*   **Conceitos-Chave:** Resposta a Incidentes (IR), gerenciamento de patches (atualizações), investigações digitais (Forense), ferramentas SIEM/SOAR, playbooks operacionais, firewalls, backups e recuperação de desastres (DRP).
*   **Foco Prático:** Manter o ambiente seguro em tempo real e garantir a resiliência operacional durante e após um ataque sofrido.

---

## 💻 8. Software Development Security (Segurança no Desenvolvimento de Software)
*Aplicar conceitos de segurança no ecossistema de desenvolvimento e criação de código (AppSec).*

*   **Conceitos-Chave:** Ciclo de Vida de Desenvolvimento de Software Seguro (SDLC), metodologias ágeis/DevSecOps, gerenciamento de configuração de software, OWASP Top 10 (principais falhas web) e riscos de código de terceiros (bibliotecas open-source).
*   **Foco Prático:** Praticar o *"Shift Left"* — empurrar a segurança para o início do desenvolvimento, evitando remediações caras quando o código já estiver em produção.

---

> 💡 **Nota de Consulta:** Para o **Curso 2**, os domínios **1 (Risk Management)**, **3 (Architecture)** e **4 (Network Security)** costumam ser os mais requisitados, pois constroem a base técnica essencial para entender o funcionamento de firewalls, criptografia e políticas de conformidade.

---

### Short definitions 
* **Security Posture(Postura de Segurança):** An organization's ability to manage ​its defense of critical assets and data and react to change.
* **Risk mitigatio:** The process of having the right procedures and rules in place to quickly reduce the impact of a risk like a breack.
* **Business continuity:** An organization's ability to maintaing their everyday productivity by stablishing risk disaster recovery plans.
* **Asset Security:** Focused on securing digital and physical assets. It's also related to the storage, maintanance, retention, and desctruction  of data.
  > Such PII and SPII.
* **Security architecture and engineering:** Focused on optimizing data security by ensuring effective tools, systems, and processes 
