# 📄 Currículo em LaTeX com VS Code

Este repositório contém a construção do meu currículo profissional utilizando **LaTeX**, com foco em **organização, reprodutibilidade e boas práticas** de versionamento e documentação.

O objetivo do projeto não é apenas gerar um currículo em PDF, mas **demonstrar como estruturar um projeto técnico simples**, aplicando conceitos comuns em ambientes DevOps, como controle de versão, build local e documentação clara.

---

## 🎯 Objetivo do projeto

- Criar um currículo profissional utilizando LaTeX
- Utilizar o VS Code como ambiente de desenvolvimento
- Versionar o projeto com Git e GitHub
- Documentar o processo para que qualquer pessoa consiga reproduzir
- Servir como **projeto de portfólio técnico**

---

## 🧠 Por que LaTeX?

O LaTeX é amplamente utilizado para documentos técnicos e acadêmicos porque:

- Garante **padronização visual**
- Separação clara entre **conteúdo e formatação**
- Excelente controle tipográfico
- Facilita versionamento (arquivos texto)
- Permite automação de builds (CI/CD)

---

## 🛠️ Tecnologias e ferramentas utilizadas

### 📌 LaTeX (MiKTeX)
Responsável por:
- Compilar o código `.tex`
- Gerar o arquivo final em PDF

Utilizei o **MiKTeX**, que permite instalar pacotes automaticamente durante a compilação.

---

### 📌 Visual Studio Code
Editor de código utilizado para:
- Escrever o arquivo `.tex`
- Gerenciar o projeto
- Integrar Git e GitHub
- Executar builds localmente

---

### 📌 Extensão LaTeX Workshop
Extensão do VS Code que:
- Integra o LaTeX ao editor
- Permite compilar o PDF com um clique
- Exibe logs de erro
- Visualiza o PDF em tempo real

---

### 📌 Strawberry Perl
O LaTeX Workshop utiliza ferramentas que dependem do **Perl**, como o `latexmk`.

O Strawberry Perl fornece:
- Ambiente Perl completo
- Compatibilidade com o `latexmk`
- Suporte ao processo de build automatizado

---

### 📌 Git e GitHub
Utilizados para:
- Controle de versão
- Histórico de alterações
- Publicação do projeto
- Compartilhamento e portfólio técnico

---

## 🔧 Requisitos para compilar o projeto

### 1️⃣ MiKTeX
Distribuição LaTeX para Windows.

- Acesse: https://miktex.org/download
- Baixe a versão adequada ao seu sistema
- Durante a instalação, marque a opção para **instalar pacotes automaticamente**

---

### 2️⃣ Strawberry Perl
Necessário para o funcionamento correto do `latexmk`.

- Acesse: https://strawberryperl.com/
- Baixe o instalador
- Instale seguindo o fluxo padrão (Next → Next)

---

### 3️⃣ Visual Studio Code
Editor de código.

- Acesse: https://code.visualstudio.com/
- Instale normalmente
- No VS Code, instale a extensão **LaTeX Workshop**
- Certifique-se de que o MiKTeX e o Strawberry Perl estejam instalados na máquina

---

## ▶️ Como compilar o currículo

### Opção 1 — Pelo VS Code (recomendado)
1. Abra a pasta do projeto no VS Code
2. Abra o arquivo `.tex`
3. Use o atalho:
   - `Ctrl + Alt + B`
   - ou clique em **Build LaTeX Project**
4. O PDF será gerado automaticamente

---

### Opção 2 — Pelo terminal
Dentro da pasta do projeto:

```bash
latexmk -pdf curriculo.tex
