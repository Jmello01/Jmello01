<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=210&section=header&text=Jo%C3%A3o%20Ricardo&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Software%20Engineer
    &descSize=20&descAlignY=60" alt="João Ricardo, Software Engineer" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/BACKEND-0D7A6F?style=for-the-badge" alt="Backend" />
  <img src="https://img.shields.io/badge/PYTHON-1E3A4A?style=for-the-badge" alt="Python" />
  <img src="https://img.shields.io/badge/JAVA-1E3A4A?style=for-the-badge" alt="Java" />
  <img src="https://img.shields.io/badge/CI%C3%8ANCIA%20DA%20COMPUTA%C3%87%C3%83O-C4A35A?style=for-the-badge" alt="Ciência da Computação" />
</p>

<p align="center">
  <a href="https://github.com/Jmello01">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=18&pause=1200&color=0D7A6F&center=true&vCenter=true&width=640&lines=Backend+com+Python+e+Java;Concorr%C3%AAncia%2C+dados+e+NLP;Aprendo+construindo;Rio+de+Janeiro%2C+Brasil" alt="Backend com Python e Java · Concorrência, dados e NLP · Aprendo construindo" />
  </a>
</p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=py,java,ts,spring,fastapi,postgres,redis,rabbitmq,docker&perline=9" alt="Python, Java, TypeScript, Spring Boot, FastAPI, PostgreSQL, Redis, RabbitMQ, Docker" />
</p>

---

## 👋 Sobre mim

Sou **Software Engineer Júnior** na DRAI Consultoria e estudante de **Ciência da Computação**. Trabalho com backend em **Python** e **Java** e aprendo construindo: quando quero entender alguma coisa, faço um projeto.

Nos projetos abaixo estudo o que mantém um sistema **correto sob carga**, e agora também como avaliar um modelo de **NLP** além de uma métrica. Antes de programar, passei 5 anos cuidando da qualidade de dados de estoque, e levo essa atenção a consistência para o código.

**Meu objetivo é chegar à arquitetura de software.**

---

## 🎯 Especialidades

```text
Backend em Python e Java            APIs REST e autenticação (JWT)
Concorrência e consistência         Lock otimista, operações atômicas
Mensageria e cache                  RabbitMQ, Redis
Bancos relacionais                  PostgreSQL, SQLite, migrations
Testes automatizados                JUnit 5, Mockito, Testcontainers, pytest
Qualidade de dados                  Validação, conciliação, tratamento
Fundamentos de ML e NLP             pandas, scikit-learn, PyTorch
```

---

## 🧰 Tech stack

**Linguagens**

<p>
  <img src="https://skillicons.dev/icons?i=py,java,ts,js" alt="Python, Java, TypeScript, JavaScript" />
</p>

**Backend e dados**

<p>
  <img src="https://skillicons.dev/icons?i=spring,fastapi,postgres,redis,rabbitmq" alt="Spring Boot, FastAPI, PostgreSQL, Redis, RabbitMQ" />
</p>

**Frontend**

<p>
  <img src="https://skillicons.dev/icons?i=react,nextjs,angular" alt="React, Next.js, Angular" />
</p>

**Infra e ferramentas**

<p>
  <img src="https://skillicons.dev/icons?i=docker,git,github,idea,vscode" alt="Docker, Git, GitHub, IntelliJ IDEA, VS Code" />
</p>

**Em estudo: machine learning**

<p>
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white" alt="Jupyter" />
</p>

---

## 🚀 Projetos em destaque

| Projeto | O que é | Stack |
|---|---|---|
| 🎟️ **[TicketFlow](https://github.com/Jmello01/ticketflow)** | Laboratório de concorrência: 1.000 threads disputam 10 ingressos. Compara sem proteção, lock otimista e Redis com decremento atômico | Java 21, Spring Boot, Redis, RabbitMQ, PostgreSQL, Docker |
| 📚 **[StudyOS](https://github.com/Jmello01/studyos)** | PWA para planejar e analisar minhas sessões de estudo, desenvolvido com TDD. *Em desenvolvimento* | Java 21, Spring Boot, PostgreSQL, Flyway, Testcontainers |
| 💸 **[Controle de Despesas API](https://github.com/Jmello01/controle-despesas-api)** | API REST com autenticação JWT, validação, tratamento de exceções e documentação Swagger, com deploy em produção | Spring Boot, JWT, PostgreSQL, Swagger, JUnit 5, Mockito |
| 🧾 **[SACT](https://github.com/Jmello01/SACT---Sistema-de-Analise-e-Calculo-Tributario)** | API de análise tributária: compara ISS com CBS + IBS (reforma tributária) e tem um motor de decisão de crédito | Python, FastAPI, SQLite, Pydantic |
| 👥 **[Next Management](https://github.com/Jmello01/next-management)** | Sistema de gestão de membros, com backend e frontend separados | Java, Spring Boot, Angular, TypeScript |

<details>
<summary><b>🔍 O que aprendi com o TicketFlow</b></summary>
<br/>

Bugs reais que encontrei e corrigi:

- O `@Retryable` envolvia uma chamada ao Redis que não é segura para repetir, e erros de banco apareciam como "estoque esgotado". Isolei a persistência em um serviço próprio.
- O cache do `open-in-view` do Spring devolvia a entidade antiga dentro da requisição. Meu teste não pegou porque rodava fora de uma requisição, e hoje há um teste que chama o endpoint de verdade.
- Publisher Confirms no RabbitMQ, para distinguir "meu código não lançou erro" de "a mensagem chegou ao broker".

Sem proteção, o cenário vendeu 1.000 ingressos e o estoque foi para -990. As outras duas abordagens vendem exatamente 10.

</details>

---

## 🏛️ Princípios de engenharia

| Antes de codar | Ao construir | Ao entregar |
|---|---|---|
| Desenho primeiro: regras de negócio, modelagem e endpoints | TDD: vejo o teste falhar antes de implementar | Testes e CI rodando antes de publicar |
| Entender o problema antes de escolher a ferramenta | Testar o que pode quebrar, não só o caminho feliz | Documentar decisões e limitações |
| Dado ruim primeiro, modelo depois | Medir contra um baseline antes de comemorar | Só publico o que consigo explicar |

> Uso assistentes de IA como mentores e para ganhar velocidade, e valido o resultado com testes e revisão de código.

---

## 🧠 Em estudo

<details>
<summary><b>🤖 Machine learning e NLP</b></summary>
<br/>

Comecei pelos fundamentos (tratamento de dados, regressão linear e logística, uma primeira rede neural em PyTorch) e agora aplico em NLP.

- **NERO** *(em breve neste perfil)*: estudo sobre como um modelo interpreta mensagens curtas em português ("Tá bom" pode ser concordância, indiferença ou irritação). Baseline contra TF-IDF + regressão logística, validação cruzada e análise de erros.
- Aprendizado até agora: com 51 mensagens, diferenças de poucos pontos são ruído, e a minha regra de anotação fazia a classe "neutra" misturar mensagens neutras e ambíguas.
- Próximos passos: mais mensagens escritas por mim e comparação com BERTimbau.

</details>

<details>
<summary><b>⚙️ Concorrência e sistemas distribuídos</b></summary>
<br/>

Locks otimistas, operações atômicas, mensageria e retry com backoff. Estudo cada conceito quebrando o sistema de propósito e escrevendo o teste que prova a correção.

</details>

<details>
<summary><b>🏗️ Arquitetura de software</b></summary>
<br/>

Meu objetivo de carreira. Estudo paradigmas de programação, SOLID, arquitetura em camadas, sistemas distribuídos e conceitos de cloud.

</details>

---

## 📊 GitHub

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Jmello01&show_icons=true&hide_border=true&count_private=true" alt="Estatísticas do GitHub" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Jmello01&layout=compact&hide_border=true" alt="Linguagens mais usadas" />
</p>

---

<p align="center">
  <i>Aprendo construindo.</i><br/>
  Se você trabalha com backend, concorrência ou NLP, vamos conversar.<br/>
  <a href="https://www.linkedin.com/in/jo%C3%A3o-mello-371a48204/">Me chama no LinkedIn</a>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=90&section=footer" alt="" />
</p>
