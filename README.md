# Sistema-de-Consulta-de-Produto-ERP-Imagens-Locais-
Sistema web em Flask para consulta rápida de produtos no banco SQL Server, exibindo descrição, DUN, EAN13 e imagem via caminho UNC. Desenvolvido para uso em intranet corporativa.

# 🔎 Sistema de Consulta de Produto (ERP + Imagens Locais)

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Flask](https://img.shields.io/badge/Flask-Web%20Framework-lightgrey)
![SQL%20Server](https://img.shields.io/badge/Database-SQL%20Server-red)
![Images](https://img.shields.io/badge/Imagens-Path%20Local-informational)

## 🧩 Sobre o projeto
Aplicação web para **pesquisa de produtos** por **código** integrada ao **SQL Server** (ERP). Exibe **código**, **descrição**, **DUN**, **EAN13** e **imagem** (carregada de um **caminho UNC** interno). Interface leve para uso em desktops na **intranet**.

> Foco inicial de desenvolvimento: **ERP CIGAM**. Compatível com qualquer ERP baseado em **SQL Server** (ajuste de queries).

## ⚙️ Funcionalidades
- 🔍 Busca rápida por **código do produto (Cd_material / PRO_CODIGO)**
- 🧾 Exibição de: **Descrição, DUN, EAN13, linha, lote** (quando aplicável)
- 🖼️ **Imagem grande** do produto (servida via caminho interno ex.: `\\\Servidor\\imagens\\...`)
- 🌐 App **web** responsivo e minimalista
- 🔒 Uso **somente em intranet** (sem dependências externas)

## 🧱 Tecnologias
Python (Flask), SQL Server (PyODBC), HTML, CSS, JS

## 📂 Estrutura
```
/app
  - main.py
  - db.py
/templates
  - base.html
  - consulta.html
/static
  - css/, js/
```

## 🔧 Configuração do SQL Server (`config.py`)
```python
DB = {
  "server": "SERVIDOR_SQL",
  "database": "CIGAM",
  "username": "USER",
  "password": "SENHA"
}
IMAGENS_BASE = r"\\\\Servidor\\imagens"
```

---

## 💡 Autor

**Desenvolvido por João Pedro Cardoso**  
💼 Consultor e desenvolvedor de soluções em automação industrial e ERP  
📧 joaopedro.vieiracardoso6@gmail.com
🌎 https://www.linkedin.com/in/joa0o/
