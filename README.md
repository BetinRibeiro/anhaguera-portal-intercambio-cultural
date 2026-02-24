#repositório anhaguera-portal-intercambio-cultural

readme_content = """
# 🎓 Portal de Intercâmbio Nacional – Universidades Brasileiras

Aplicação web desenvolvida para busca de instituições de ensino superior no Brasil, utilizando API pública internacional.

Projeto publicado via **GitHub Pages**.

🔗 Repositório:
https://github.com/BetinRibeiro/anhaguera-portal-intercambio-cultural

---

## 🌐 Acesso Online (GitHub Pages)

Se já estiver ativo:

https://BetinRibeiro.github.io/anhaguera-portal-intercambio-cultural/

Caso precise ativar:

1. Vá em **Settings**
2. Clique em **Pages**
3. Em *Source* selecione:
   - Branch: `main`
   - Folder: `/root`
4. Salve

---

## 📌 Objetivo do Projeto

Criar um portal moderno, responsivo e intuitivo para:

- Pesquisar universidades brasileiras
- Filtrar por nome, sigla ou região
- Facilitar acesso a sites oficiais
- Servir como base para projetos acadêmicos e extensão cultural

---

## 🚀 Funcionalidades

✅ Busca livre por nome da instituição  
✅ Filtro automático limitado ao Brasil  
✅ Integração com API pública (Hipolabs Universities API)  
✅ Interface moderna e responsiva  
✅ Cards dinâmicos com:
- Nome da universidade
- Estado (quando disponível)
- Domínio institucional
- Link direto para o site oficial  
✅ Skeleton loading (efeito de carregamento)  
✅ Tratamento de erros de conexão  
✅ Layout adaptável para dispositivos móveis  

---

## 🛠 Tecnologias Utilizadas

- HTML5
- CSS3 (custom properties + design system próprio)
- JavaScript Vanilla (ES6+)
- Fetch API
- Google Fonts (Plus Jakarta Sans)
- Font Awesome (ícones)
- GitHub Pages (deploy)

---

## 🔎 API Utilizada

Hipolabs Universities API  
Endpoint utilizado:

http://universities.hipolabs.com/search?country=Brazil&name=

A API retorna:

- Nome da instituição
- Estado (quando disponível)
- Domínio
- Página oficial

---

## 📂 Estrutura do Projeto

anhaguera-portal-intercambio-cultural/
│
├── index.html
└── README.md

Projeto 100% front-end.

---

## 💻 Como Executar Localmente

Clone o repositório:

git clone https://github.com/BetinRibeiro/anhaguera-portal-intercambio-cultural.git

Entre na pasta:

cd anhaguera-portal-intercambio-cultural

Abra:

index.html

Ou rode um servidor local:

python -m http.server 8000

---

## 📱 Responsividade

- Desktop
- Tablet
- Mobile
- Layout adaptável com media queries
- Navbar fixa (sticky)
- Grid automático com auto-fill

---

## 🎯 Possíveis Melhorias Futuras

- Filtro por estado (UF)
- Paginação de resultados
- Favoritar universidades
- Exportar lista em PDF
- Sistema de login
- Banco de dados próprio
- Versão PWA (instalável)
- HTTPS obrigatório na API (evitar bloqueio CORS)

---

## 👨‍💻 Autor

**Betin Ribeiro**

GitHub:
https://github.com/BetinRibeiro

---

## 📄 Licença

Projeto acadêmico / educacional.
Livre para uso em fins institucionais e de aprendizado.
"""

import pypandoc

output_file = "/mnt/data/README_anhaguera_portal_intercambio_cultural.md"

pypandoc.convert_text(
    readme_content,
    'md',
    format='md',
    outputfile=output_file,
    extra_args=['--standalone']
)

output_file
