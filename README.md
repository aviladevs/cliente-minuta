
# Cliente Minuta - Avila Transportes

Sistema simples para cadastro de cliente com geração de minuta em PDF.

## 🚀 Funcionalidades

- Formulário no navegador
- Backend em Node.js (Express)
- Geração de PDF com Puppeteer
- Deploy automatizado com Azure DevOps
- Pronto para publicação no Azure App Service

---

## 📁 Estrutura do Projeto

```
cliente-minuta/
├── public/                    # Formulário HTML
├── templates/                # Template HTML da minuta
├── output/                   # Pasta onde o PDF é gerado
├── server.js                 # Servidor Express
├── package.json              # Configuração Node.js
├── azure-pipelines.yml       # Pipeline Azure DevOps
```

---

## 📦 Como rodar localmente

```bash
npm install
node server.js
```

Acesse: `http://localhost:3000`

---

## ☁️ Deploy no Azure

### 1. Crie o repositório no Azure DevOps
Suba todos os arquivos deste projeto com:
```bash
git init
git remote add origin <URL do repositório>
git add .
git commit -m "Deploy inicial"
git push -u origin main
```

### 2. Crie o App Service no Azure
Você pode usar o script `deploy.azcli` abaixo ou criar manualmente pelo portal.

### 3. Configure o deploy contínuo
No portal Azure:
- Vá em **Centro de Implantação** do seu App Service
- Selecione Azure Repos
- Escolha seu repositório e branch `main`

---

## 📄 PDF gerado

O PDF é gerado e baixado automaticamente no navegador após o envio do formulário.
