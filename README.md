
# 🚀 Projeto Node.js com CI/CD e Docker

Este projeto foi criado para demonstrar uma pipeline de CI/CD funcional usando GitHub Actions. Ele inclui testes automatizados com Jest e o deploy automático de uma imagem Docker no Docker Hub.

---

## 📋 O que foi feito

✅ Aplicação simples em Node.js para testes na pipeline
✅ Testes automatizados usando Jest  
✅ Pipeline CI/CD com GitHub Actions  
✅ Deploy automático para o Docker Hub via Dockerfile

---

## ⚙️ Tecnologias usadas

- Node.js
- Jest
- Docker
- GitHub Actions

---

## 🔄 Como funciona a pipeline

Toda vez que alguém faz um **push no branch `main`**, a pipeline faz automaticamente:

1. 🧪 **Instala as dependências**
2. 🔬 **Roda os testes**
3. 🐳 **Gera a imagem Docker**
4. 🚀 **Faz push da imagem pro Docker Hub**

---

## 🐳 Como rodar com Docker

Você pode testar a aplicação usando Docker com os comandos:

```bash
docker pull joaogivisiez/meu-app-node:latest
docker run -p 3000:3000 joaogivisiez/meu-app-node:latest
```

---

## 🧪 Como rodar localmente

Se quiser rodar sem Docker:

```bash
git clone https://github.com/joao-givisiez/Projeto-Comp.git (clonagem do repositorio para git)
cd Projeto-Comp
npm install
npm test
npm start
```

---

## 📁 Estrutura principal

```
Projeto-Comp/
├── src/              # Código da aplicação
├── tests/            # Testes com Jest
├── Dockerfile
├── package.json

.github/
├──workflows/
        ├──ci-cd.yml
```

---

## 💡 Sobre o projeto

Esse repositorio contem uma pipeline com praticas de devops, sendo um pipeline de integraçao continua e entrega continua. Ela foi desenvolvida por mim(joao vitor)
afim de resolver um problema de infraestrutura de entrega de uma determinda empresa. O doploy pode ser feito em varios tipos de ambientes como locais ou web, mas 
visando o projeto como um problema "nao ofcial", optei por descarregar a a imagem no meu repositorio de imagens Docker Hub. Finalizo resaltando que a alteraçao de deploy 
esta estrategicamenbte definida para ser simples e evitar grandes mudanças no projeto!
---

## 🙋 Quem fez?

Desenvolvedor @joao.givisez_
