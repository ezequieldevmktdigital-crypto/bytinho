# 🤖 DIO Agent

> Seu mentor com Inteligência Artificial para aprender mais e melhor na [DIO](https://dio.me).

O **DIO Agent** é um agente de IA que acompanha você na sua jornada de estudos. Ele conhece as experiências da DIO (Bootcamps, Formações, Cursos, Desafios e muito mais) e ajuda você a estudar, praticar e planejar a sua carreira.

Você não precisa saber programar nem instalar nada complicado. Em **3 passos**, o seu mentor está pronto para usar.

---

## ✨ Três palavras para começar

- 🧠 **Agente de IA:** um chatbot responde perguntas. Um *agente* vai além: lê, planeja e executa passos para ajudar você a alcançar um objetivo. É a diferença entre alguém que explica o caminho e alguém que caminha junto com você.
- 🖥️ **Harness:** é o programa onde o agente roda. O agente é o mentor, e o harness é a sala onde vocês se encontram. O mesmo mentor atende em salas diferentes, por isso o DIO Agent funciona em vários harnesses.
- 🧩 **Skill:** é uma habilidade do agente, descrita em um guia passo a passo. Você não precisa chamar a skill: o agente percebe o que você precisa e usa a certa sozinho.

Esses e outros termos estão no [Glossário](docs/glossary.md).

---

## 🚀 Comece em 3 passos

### 1️⃣ Instale um harness

Recomendamos o **Google Antigravity**, que tem limites de uso generosos para quem está começando. Mas qualquer harness da lista funciona: escolha um e siga a instalação da documentação oficial dele.

| Harness | Documentação oficial |
|---------|----------------------|
| Google Antigravity (recomendado) | https://antigravity.google/docs |
| Claude Code | https://code.claude.com/docs |
| Codex | https://developers.openai.com/codex |
| OpenCode | https://opencode.ai/docs |
| Hermes | https://hermes-agent.nousresearch.com/docs |

### 2️⃣ Baixe o DIO Agent e abra no harness

Baixe este repositório do jeito mais simples para você:

- **Com Git:** no terminal, rode `git clone https://github.com/digitalinnovationone/dio-agent.git`
- **Sem Git:** no topo desta página, clique no botão verde **Code**, depois em **Download ZIP**, e extraia a pasta.

Depois, abra no harness a pasta do projeto, a que tem o arquivo `AGENTS.md` (pelo Git, ela se chama `dio-agent`; pelo .zip, `dio-agent-main`). O harness lê esse arquivo sozinho, e o agente já sabe quem é: o seu mentor de estudos da DIO.

### 3️⃣ Converse

Fale naturalmente, com as suas palavras. Nas primeiras vezes, vale usar um dos [modelos de prompt](#-modelos-de-prompt) abaixo: quanto mais contexto você dá, melhor o agente ajuda.

---

## 🧩 As skills do agente

| Skill | Para que serve | Experimente pedir |
|-------|----------------|-------------------|
| [Plano de estudos](skills/study-plan/SKILL.md) | Organiza o que estudar, em que ordem e em quanto tempo | "Quero concluir este Bootcamp em 2 meses, me ajuda?" |
| [Destravar desafio](skills/unblock-challenge/SKILL.md) | Conduz você até a solução de um desafio, sem dar a resposta pronta | "Travei nesse desafio, me ajuda?" |
| [Explicar conceito](skills/explain-concept/SKILL.md) | Explica conceitos de forma simples, com analogias e exemplos | "Não entendi o que é uma API." |
| [Pesquisa na web](skills/web-search/SKILL.md) | Responde dúvidas atuais (versões, lançamentos, mercado) com fontes citadas | "Qual a versão estável do Node hoje?" |
| [Revisão de portfólio](skills/portfolio-review/SKILL.md) | Dá feedback sobre o seu portfólio e GitHub antes de buscar vagas | "O que falta no meu GitHub para uma vaga júnior?" |
| [Caminho AI Builder](skills/ai-builder-path/SKILL.md) | Ajuda você a escolher o próximo passo na Carreira AI Builder | "Qual Formação AI Builder combina comigo?" |
| [Laboratório de pentest](skills/pentest-lab/SKILL.md) | Monta um laboratório local de segurança em VMs isoladas (opcional, avançado) | "Quero montar um laboratório de pentest em casa." |
| [Análise de vulnerabilidades](skills/pentest-vulnerability/SKILL.md) | Explica um achado de scan, o impacto e a correção (opcional, avançado) | "Encontrei essa vulnerabilidade no meu lab, me ajuda?" |

A pesquisa na web usa a busca do seu harness. Se ele não tiver busca própria, veja [como conectar o You.com](docs/youcom-mcp.md), que tem uma opção gratuita.

---

## 📝 Modelos de prompt

Copie, preencha o que está entre colchetes e envie. Não precisa de formato perfeito: o agente pede mais detalhes se precisar.

**🗺️ Plano de estudos**

```
Quero montar um plano de estudos.
- Meu objetivo: [ex: ser dev back-end, concluir um Bootcamp]
- O que quero fazer na DIO: [link ou nome do Bootcamp, Formação, Aceleração ou Carreira]
- O que já tenho: [um plano de ação ou de estudos, se tiver]
- Meu nível hoje: [iniciante, intermediário, avançado]
- Tempo disponível: [ex: 1 hora por dia, de segunda a sexta]
```

**🔓 Destravar desafio**

```
Estou travado em um Desafio de [Código, Projeto ou Criativo] da DIO.
- O que o desafio pede: [cole o enunciado ou, no Desafio de Projeto, o link do repositório do desafio]
- Onde eu travei: [explique o ponto da dificuldade]
- Meu código ou repositório: [cole o código ou o link, se tiver]
Me ajuda a destravar sem dar a resposta pronta.
```

**💡 Explicar conceito**

```
Me explica o conceito de [ex: API, laço de repetição, herança].
- Meu nível: [nunca vi, já ouvi falar, quero aprofundar]
```

**🧭 Caminho AI Builder**

```
Quero escolher meu próximo passo na Carreira AI Builder.
- O que quero construir com IA: [ex: um produto para o meu negócio, um software, agentes que automatizam processos, ainda não sei]
- Minha experiência com programação: [nenhuma, o básico, trabalho com desenvolvimento]
- Meu objetivo: [ex: mudar de carreira, tirar uma ideia do papel]
```

**🛡️ Laboratório de pentest (opcional, avançado)**

```
Quero montar um laboratório local de pentest.
- Meu nível com redes/Linux: [nunca estudei, sei o básico, já pratico]
- Já usei VirtualBox: [sim, não]
- O que quero aprender: [ex.: reconhecimento, análise de vulnerabilidades]
- Confirme que vou usar só a rede 192.168.56.0/24
```

---

## 🛡️ GuardIA: laboratório de segurança

Se você quiser estudar segurança, o DIO Agent entra no **modo GuardIA**: um mentor que ensina testes de penetração em um laboratório local, isolado e criado por você.

Antes de qualquer exercício, o agente lê as [regras de escopo](docs/pentest-scope.md) e valida o alvo. Só a rede `192.168.56.0/24` (VirtualBox Host-Only) e o loopback são autorizados. A rede do seu Wi-Fi, a Internet e qualquer sistema de terceiro estão fora de escopo — ponto final.

Este é um conteúdo **opcional e avançado**. Se você está começando em tecnologia, siga primeiro o plano de estudos. O laboratório não é necessário para as outras skills.

O guia de montagem está em [`skills/pentest-lab/scripts/lab-setup.md`](skills/pentest-lab/scripts/lab-setup.md). Para checar o ambiente sem contatar nenhum alvo:

```
python skills/pentest-lab/scripts/env_check.py
```

---

## 🔄 Mantenha o DIO Agent atualizado

O DIO Agent evolui com o tempo. Se você usou Git, rode `git pull` no terminal, dentro da pasta (ou peça para o próprio agente rodar). Se baixou o .zip, baixe de novo.

---

## 🗂️ Estrutura do repositório

```
dio-agent/
├── README.md                Este guia
├── AGENTS.md                Definição do agente (lida pelo harness)
├── CLAUDE.md                Atalho para o Claude Code
├── agent/
│   ├── persona.md           A personalidade e o tom do agente
│   └── knowledge/           O que o agente sabe sobre a DIO
│       └── persona-guardia.md   O modo GuardIA (segurança)
├── skills/                  Uma pasta por skill, cada uma com o seu SKILL.md
│   ├── pentest-lab/         Laboratório local (opcional)
│   │   ├── scripts/         scope_guard.py, env_check.py, lab-setup.md
│   │   ├── evidence/        Modelos de evidência
│   │   ├── scans/           Modelos de resultado de scan
│   │   └── report/          Modelo de relatório final
│   └── pentest-vulnerability/   Análise de vulnerabilidades (opcional)
└── docs/
    ├── glossary.md          Glossário de termos
    ├── youcom-mcp.md        Como conectar a busca do You.com
    └── pentest-scope.md     Escopo e autorização do laboratório
```

---

## 🤝 Contribua

Tem uma ideia de skill? Veja [como criar uma skill](skills/README.md) e abra um pull request.

---

## 💬 Sobre este projeto

O DIO Agent foi criado para acompanhar você nos Bootcamps e Formações da DIO. A ideia é simples: aprender na era da IA fica mais fácil quando você tem um mentor disponível a qualquer hora.

Bons estudos, e vem com a gente. 🚀

---

## 📓 Registro de atividade (simulado)

> Registro fictício, criado apenas para validar o padrão de documentação do GuardIA. Nenhuma ferramenta foi executada e nenhuma verificação técnica foi feita.

| Campo | Valor |
|-------|-------|
| ID da atividade | LAB-001 |
| Nome | Teste de validação documental |
| Ambiente | Laboratório fictício |
| Objetivo | Verificar a estrutura de registro do GuardIA |
| Status | CONCLUÍDO |
| Resultado | Teste simulado de documentação, sem execução técnica |
| Vulnerabilidades | Nenhuma avaliada |
| Recomendação | Nenhuma |
