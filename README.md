# Projeto de Estudo: Cronômetro com Git e Feature Branch Workflow

Este repositório foi criado para praticar e consolidar o uso de Git e GitHub com um fluxo baseado em branches de funcionalidades (_Feature Branch Workflow_), aplicando os conhecimentos em um pequeno projeto de cronômetro (Stopwatch).

## 🧠 Objetivo

- Desenvolver uma aplicação funcional de cronômetro usando HTML, CSS e JavaScript.
- Simular um fluxo de trabalho com feature branches.
- Aplicar deploy automático com **Netlify** após integrações no `main`.

---

## 📁 Estrutura do Projeto

O projeto é composto por arquivos estáticos:

- `index.html` – estrutura da interface do cronômetro
- `style.css` – estilo da interface
- `script.js` – lógica de funcionamento do cronômetro

---

## 🧪 Fluxo de Trabalho Aplicado

### 🟢 1. `main`

Branch principal do projeto, mantido limpo e pronto para deploy.

### 🌿 2. `interface`

Branch criado a partir do `main` para desenvolvimento da interface HTML e CSS.

- Criado com: `git checkout -b interface main`
- Contém toda a estrutura visual do cronômetro.

### 🌿 3. `script`

Branch criado a partir do `interface` para implementação da lógica JavaScript.

- Criado com: `git checkout -b script interface`
- Inclui funcionalidades de iniciar, pausar, resetar e contar tempo.

---

## 🔄 Integração e Deploy

- Os branches foram integrados ao `main` via **Pull Requests** no GitHub.
- Após cada merge, o **Netlify** realizou o deploy automático da nova versão.

### 🔗 Projeto Online

🌐 **[https://raci-stopwatch.netlify.app/](https://raci-stopwatch.netlify.app/)**

---

## 🧹 Limpeza Final

Após os merges, os branches foram removidos:

```bash
# Deleção local
git branch -d interface
git branch -d script

# Deleção remota (GitHub)
git push origin --delete interface
git push origin --delete script
```

## 📚 Aprendizados

- Criação e gerenciamento de branches por funcionalidade.
- Aplicação prática do Git em projetos reais (mesmo solo).
- Experiência com deploy contínuo via Netlify.
- Exercício de controle de versão em projetos modulares (interface e lógica separados).

---

## 📌 Tecnologias

- Git & GitHub
- HTML / CSS / JavaScript
- Netlify (Deploy Automático)

---

## 🚀 Resultado

Este projeto ajudou a consolidar o uso do Git com um fluxo organizado de desenvolvimento.  
O conhecimento adquirido será base para projetos futuros mais complexos.
