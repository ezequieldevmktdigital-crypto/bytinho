# 🛡️ GuardIA

> Seu agente inteligente de Segurança da Informação para aprender, analisar, praticar e evoluir em Cibersegurança.

O **GuardIA** é um agente de Inteligência Artificial especializado em Segurança da Informação, Cibersegurança, análise de vulnerabilidades, Pentest, redes, sistemas Linux e Windows, aplicações Web e defesa cibernética.

Ele acompanha você na jornada de aprendizado e prática em segurança, ajudando a compreender conceitos, planejar avaliações, analisar ferramentas, investigar vulnerabilidades, desenvolver habilidades técnicas e documentar cada atividade.

O GuardIA foi projetado para atuar como um mentor técnico e assistente de segurança, combinando conhecimento, instruções especializadas e metodologias organizadas.

Você pode utilizá-lo no Hermes Agent, dentro do seu ambiente de desenvolvimento, para estudar, analisar projetos, trabalhar em laboratórios controlados e organizar suas avaliações de segurança.

---

## ✨ Três conceitos para começar

- 🧠 **Agente de IA:** um chatbot responde perguntas. Um agente vai além: interpreta objetivos, consulta referências, planeja etapas e utiliza ferramentas disponíveis para auxiliar na realização de tarefas. O GuardIA atua como seu assistente de segurança, orientando investigações e análises.

- 🖥️ **Harness:** é o ambiente onde o agente funciona, acessa suas instruções, interage com ferramentas e executa tarefas. O Hermes é o ambiente utilizado neste projeto para operar o GuardIA.

- 🧩 **Skill:** é uma habilidade especializada, descrita por instruções que orientam o agente a realizar determinado tipo de tarefa. As skills ajudam o GuardIA a seguir metodologias específicas sem precisar concentrar todas as instruções em um único arquivo.

---

## 🚀 Comece em 3 passos

### 1️⃣ Instale e configure o Hermes

O GuardIA utiliza o Hermes Agent como ambiente de execução.

Instale e configure o Hermes seguindo a documentação oficial:

https://hermes-agent.nousresearch.com/docs/

Configure o provedor de IA, modelo, terminal backend e ferramentas conforme seu ambiente.

### 2️⃣ Abra o projeto no VS Code

Abra no VS Code a pasta raiz do projeto GuardIA.

O agente utiliza arquivos de instrução, conhecimento e skills para orientar seu comportamento.

Estrutura principal:

- `agent/` — arquivos de identidade, conhecimento e contexto.
- `agent/knowledge/` — referências técnicas utilizadas para fundamentar respostas.
- `skills/` — procedimentos especializados para tarefas específicas.
- `README.md` — documentação central do projeto.

### 3️⃣ Converse com o GuardIA

Fale naturalmente.

Você pode pedir explicações, solicitar análises, estudar ferramentas, elaborar planos de testes, entender vulnerabilidades ou montar laboratórios.

Quanto mais contexto você fornecer — objetivo, ambiente, nível de conhecimento e restrições — melhor será a orientação.

---

## 🧩 Conhecimento e skills

O GuardIA utiliza referências e instruções especializadas para manter suas respostas organizadas e consistentes.

| Módulo | Local | Para que serve |
|---|---|---|
| Security Basics | `agent/knowledge/security-basics/` | Referência de conceitos, fundamentos, terminologia e boas práticas de segurança |
| Pentest Analysis | `agent/skills/pentest-analysis/` | Metodologia para organizar avaliações, analisar resultados, registrar achados e documentar testes |

### 📚 Security Basics

A base `security-basics` é a referência de conhecimento do GuardIA para assuntos de Segurança da Informação.

Ela pode reunir conteúdos como:

- Fundamentos de Cibersegurança.
- Redes e protocolos.
- Linux e Windows.
- Vulnerabilidades.
- Segurança Web.
- Autenticação e autorização.
- Criptografia.
- OSINT.
- Segurança ofensiva e defensiva.
- Hardening.
- Ferramentas de segurança.
- Glossário técnico.

O agente deve consultar os materiais relevantes dessa base ao responder questões de segurança, priorizando as referências disponíveis e identificando quando utilizar conhecimento complementar.

### 🛠️ Pentest Analysis

A skill `pentest-analysis` orienta o GuardIA na organização de avaliações técnicas.

Seu propósito é:

- Planejar testes de segurança.
- Definir e respeitar o escopo.
- Identificar ativos autorizados.
- Organizar etapas de análise.
- Interpretar resultados de ferramentas.
- Diferenciar suspeitas de vulnerabilidades confirmadas.
- Registrar evidências.
- Classificar riscos.
- Recomendar correções.
- Documentar atividades no README.

A skill deve ser utilizada em avaliações autorizadas, laboratórios locais e ambientes controlados.

---

## 🎯 O que você pode fazer com o GuardIA?

| Área | Aplicação |
|---|---|
| 🔎 Reconhecimento | Compreender a superfície de ataque e informações disponíveis |
| 🌐 Redes | Estudar protocolos, portas, serviços e arquitetura de redes |
| 🐧 Linux | Aprender comandos, permissões, serviços e hardening |
| 🪟 Windows | Analisar configurações, serviços, permissões e segurança |
| 🕸️ Web Security | Estudar aplicações Web, sessões, APIs e vulnerabilidades |
| 🧪 Pentest | Planejar e realizar testes autorizados em laboratórios |
| 🛡️ Defesa | Aprender prevenção, detecção, mitigação e resposta |
| 📊 Vulnerabilidades | Analisar CVEs, impacto, severidade e correções |
| 📁 Código | Revisar códigos em busca de problemas de segurança |
| 📝 Relatórios | Documentar testes, evidências, riscos e recomendações |
| 🧠 Aprendizado | Construir conhecimento técnico de forma progressiva |

---

## 📝 Modelos de prompt

Copie, adapte e envie ao GuardIA. Você não precisa escrever prompts complexos: descreva o que deseja aprender ou analisar.

### 💡 Explicar um conceito de segurança

```text
GuardIA, quero estudar um conceito de Segurança da Informação.

- Assunto: [ex.: SQL Injection, MITM, DNS, firewall]
- Meu nível: [iniciante, intermediário ou avançado]
- Objetivo: [entender, praticar, preparar uma auditoria]

Explique o conceito, como funciona, exemplos didáticos,
riscos, formas de identificar e medidas de prevenção.

Consulte sua base security-basics antes de responder.
```

### 🔍 Analisar uma vulnerabilidade

```text
GuardIA, quero analisar uma vulnerabilidade.

- Vulnerabilidade: [nome ou CVE]
- Sistema afetado: [software, versão ou laboratório]
- Evidência disponível: [resultado de scan, log ou descrição]
- Objetivo: [compreender o impacto e a correção]

Explique a vulnerabilidade, condições necessárias,
impactos, formas seguras de validação e recomendações.

Diferencie informações confirmadas de hipóteses.
```

### 🧪 Montar um laboratório de Pentest

```text
GuardIA, quero montar um laboratório de Pentest local.

- Meu nível: [iniciante, intermediário ou avançado]
- Virtualizador: [VirtualBox, VMware ou outro]
- Sistemas disponíveis: [Kali, Ubuntu, Windows, máquinas vulneráveis]
- Objetivo: [redes, Web, serviços, análise de vulnerabilidades]
- Escopo: somente máquinas virtuais próprias e rede isolada

Monte um plano de laboratório, explique a arquitetura,
os requisitos, a rede, os riscos e as etapas de configuração.

Não execute alterações antes de apresentar o plano e aguardar minha aprovação.
```

### 🖥️ Aprender uma ferramenta no terminal

```text
GuardIA, quero aprender uma ferramenta de segurança.

- Ferramenta: [Nmap, Wireshark, WPScan, ZAP etc.]
- Sistema: [Kali Linux, Ubuntu, Windows]
- Meu nível: [iniciante, intermediário, avançado]
- Objetivo: [o que desejo aprender]

Explique a ferramenta, seus recursos, parâmetros,
comandos de laboratório, resultados esperados,
interpretação e medidas defensivas.

Utilize somente alvos locais ou explicitamente autorizados.
```

### 🛡️ Auditoria de segurança

```text
GuardIA, quero planejar uma auditoria de segurança.

- Ambiente: [laboratório, sistema próprio ou ambiente autorizado]
- Alvo: [identificação do ativo]
- Escopo autorizado: [IPs, domínios ou sistemas]
- Objetivo: [verificar segurança, configurações ou exposição]
- Restrições: [limites de teste]

Crie um plano organizado por fases, com ferramentas,
objetivos, riscos, critérios de validação e documentação.

Não execute testes ativos antes de validar o escopo e obter minha aprovação.
```

### 📋 Documentar um resultado

```text
GuardIA, analise o resultado deste teste e documente.

- Teste: [nome]
- Alvo: [ativo autorizado]
- Ferramenta: [nome]
- Resultado: [cole a saída]

Interprete os resultados, identifique possíveis riscos,
diferencie achados confirmados de suspeitas e falsos positivos,
recomende correções e prepare um registro para o README.md.

Não invente resultados e preserve a documentação existente.
```

---

## 🛡️ GuardIA Lab — Laboratório de Segurança

O GuardIA possui uma proposta de utilização prática para aprendizado de segurança cibernética por meio de laboratórios controlados.

O laboratório é destinado ao estudo de redes, sistemas, serviços, vulnerabilidades e técnicas de análise de segurança em ambientes próprios ou explicitamente autorizados.

### Ambiente recomendado

- Kali Linux — estação de análise.
- Ubuntu Server — servidor de laboratório.
- Windows — laboratório de auditoria e administração.
- OWASP Juice Shop — aplicação Web vulnerável para aprendizado.
- Metasploitable — sistema intencionalmente vulnerável para treinamento.
- VirtualBox — virtualização e isolamento das máquinas.

### Regras do laboratório

- Utilizar máquinas virtuais próprias.
- Isolar a rede do laboratório.
- Definir os alvos antes dos testes.
- Não utilizar redes de terceiros.
- Não testar sistemas públicos sem autorização.
- Evitar ações destrutivas.
- Registrar comandos e resultados.
- Documentar evidências.
- Restaurar snapshots quando necessário.

O laboratório é opcional e recomendado para quem deseja aprofundar os estudos práticos de Segurança da Informação.

---

## 📑 Documentação das avaliações

O GuardIA utiliza documentação em Markdown para manter um histórico organizado das avaliações e atividades realizadas.

A documentação deve registrar:

- Objetivo do teste.
- Escopo e autorização.
- Ambiente.
- Data e horário.
- Metodologia.
- Ferramentas.
- Comandos executados.
- Resultados observados.
- Evidências.
- Vulnerabilidades confirmadas.
- Falsos positivos.
- Classificação de riscos.
- Recomendações.
- Retestes.
- Conclusão.

O README deve preservar o histórico existente, sem apagar resultados anteriores, e distinguir claramente testes planejados, executados e simulados.

---

## 📂 Estrutura do projeto

```text
GuardIA/
├── README.md
├── agent/
│   ├── knowledge/
│   │   └── security-basics/
│   │       └── [referências de segurança]
│   └── skills/
│       └── pentest-analysis/
│           ├── README.md
│           └── SKILL.md
├── docs/
│   └── [documentação complementar]
├── evidencias/
│   └── [evidências sanitizadas]
├── scans/
│   └── [resultados de análises autorizadas]
└── relatorios/
    └── [relatórios de segurança]
```

Os diretórios de evidências, scans e relatórios podem ser adicionados conforme a necessidade do projeto.

---

## 🔄 Evolução do GuardIA

O GuardIA é um projeto modular. Novos conhecimentos, instruções e habilidades podem ser adicionados gradualmente.

Possíveis módulos futuros:

- Reconhecimento e OSINT.
- Network Recon.
- Web Security.
- Linux Security.
- Windows Security.
- Vulnerability Analysis.
- Malware Analysis — análise controlada.
- Cloud Security.
- Docker Security.
- Incident Response.
- Report Engine.
- Lab Manager.

Cada novo módulo deve possuir um objetivo claro, instruções próprias e limites operacionais.

---

## 🤝 Contribua para o conhecimento

O conhecimento do GuardIA pode evoluir por meio da adição de novas referências, documentação técnica, metodologias e skills.

Ao adicionar materiais:

- Prefira fontes confiáveis.
- Organize por assunto.
- Evite duplicidade.
- Identifique materiais desatualizados.
- Não inclua credenciais ou dados sensíveis.
- Diferencie documentação de procedimentos executáveis.

---

## 💬 Sobre o GuardIA

O GuardIA foi concebido para ser um parceiro de aprendizado e análise em Segurança da Informação.

Seu propósito é transformar conhecimento técnico em compreensão, prática controlada e melhoria de segurança.

Mais do que executar ferramentas, o GuardIA busca ensinar como interpretar resultados, compreender riscos, validar evidências e corrigir vulnerabilidades.

**Investigue com método. Aprenda com profundidade. Valide com evidências. Documente cada etapa.**

🛡️ **GuardIA — Inteligência aplicada à Segurança.**
