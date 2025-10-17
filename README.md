# 🧭 Desafio AWS Step Functions

Este repositório contém os conceitos e práticas desenvolvidas durante o módulo **AWS Step Functions**, abordando a criação de **workflows automatizados** e a **integração com outros serviços da AWS**.

---

## 📂 Estrutura de diretórios

- **images/**
  - `Diagrama.jpg` — Diagrama criado no **AWS Step Functions** representando o fluxo de validação do pedido.  
  - `Criacao_diagrama.jpg` — Imagem da tela no momento da criação do diagrama no console da AWS.

- **codigo/**
  - `codigo_json.txt` — Código **JSON** utilizado na definição do diagrama (State Machine).

---

## ⚙️ AWS Step Functions

O **AWS Step Functions** é um serviço de **orquestração serverless** que permite coordenar componentes de aplicações distribuídas e microsserviços por meio de **workflows visuais**.  
Ele gerencia a lógica e o estado das aplicações, reduzindo a necessidade de código manual e acelerando o desenvolvimento de soluções automatizadas.  

Com o Step Functions, é possível criar **máquinas de estado** que definem etapas e fluxos de execução, facilitando a automação de processos complexos e a integração de diversos serviços da AWS.

---

## 🚀 Desafio proposto

Foi criado, utilizando o serviço **AWS Step Functions**, o **fluxo de validação de um pedido**, conforme ilustrado no diagrama disponível em:  
[📊 `images/Diagrama.jpg`](images/Diagrama.jpg)

### 🔁 Fluxo de execução

1. O **AWS Lambda** valida o pedido com base em `pedido_id` e `valor`.  
2. Caso ocorra algum erro na validação, o **Amazon SNS** é acionado para enviar uma notificação com os detalhes do erro.

O código utilizado na definição do diagrama está disponível em:  
[`codigo/codigo_json.txt`](codigo/codigo_json.txt)

---

## 🧩 Outros conceitos utilizados no desafio

### **AWS Lambda**
O **AWS Lambda** é um serviço de computação **serverless** que executa código (funções Lambda) em resposta a eventos, sem necessidade de provisionar ou gerenciar servidores.  
Ele escala automaticamente conforme a demanda e permite criar soluções altamente eficientes e econômicas.

---

### **Amazon SNS (Simple Notification Service)**
O **Amazon SNS** é um serviço de **mensageria assíncrona**, altamente **disponível, escalável e seguro**, que facilita o envio de notificações entre **aplicativos distribuídos**, **microserviços** e **usuários finais**.  
Ele permite o envio de mensagens para múltiplos canais, como **notificações push**, **mensagens SMS**, **e-mails** e integrações com outros serviços da AWS, como **Amazon SQS** e **AWS Lambda**.

---

### ✅ **Resumo**
Este projeto demonstra o uso integrado de **AWS Step Functions**, **AWS Lambda** e **Amazon SNS** para construir um workflow automatizado de validação de pedidos, reforçando os conceitos aprendidos no módulo de orquestração de processos serverless.
