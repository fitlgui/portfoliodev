# Portfólio — Guilherme Fitl de Carvalho

## Visão Geral
Este repositório contém o portfólio pessoal de Guilherme Fitl (Guilherme Fitl de Carvalho), um Desenvolvedor Front‑End especializado em Angular e Tailwind CSS. A página é uma aplicação estática (HTML/CSS/JS) cuidadosamente estilizada com animações modernas, efeitos visuais e seções que descrevem experiência, projetos e formas de contato.

O objetivo deste projeto é apresentar habilidades, projetos relevantes (incluindo um e‑commerce publicado em https://tpstintas.com.br) e fornecer um ponto de contato profissional para recrutadores e clientes.

---

## Principais Características
- Design moderno com gradientes animados, glassmorphism e transições suaves
- Seções: Home, Sobre, Experiência, Projetos, Contato
- Projetos em destaque com links externos (ex.: tpstintas.com.br)
- Formulário de contato com fallback via mailto
- Navegação responsiva (header fixo com menu mobile)
- Pequenas melhorias de acessibilidade (focus states, navegação por teclado)

---

## Tecnologias
- HTML5
- CSS (Tailwind via CDN + custom CSS)
- JavaScript vanilla para interatividade
- Flowbite (componentes utilitários)
- Fontes Google (Inter)

---

## Estrutura do Projeto
```
portfolio/
├─ index.html        # Página principal do portfólio
├─ Profile.svg       # Imagem de perfil (substitua pela sua foto)
└─ README.md         # Este arquivo
```

> Observação: Se você adicionar imagens, coloque-as na mesma pasta ou em uma subpasta `assets/` e atualize os caminhos no `index.html`.

---

## Como visualizar localmente (Windows - PowerShell)
Você pode abrir `index.html` diretamente no navegador, mas para um comportamento mais próximo de um servidor web (melhor para links relativos), recomendo iniciar um servidor estático.

1) Usando Python (se tiver instalado):

```powershell
cd 'C:\Users\00558374\Documents\fitl\portfoliodev'
python -m http.server 8000
# Abra no navegador: http://localhost:8000
```

2) Alternativa com Node (http-server):

```powershell
npm install -g http-server
cd 'C:\Users\00558374\Documents\fitl\portfoliodev'
http-server -p 8000
# Abra no navegador: http://localhost:8000
```

---

## Personalizações recomendadas
- Substitua `Profile.svg` por uma foto profissional (mesmo tamanho recomendado: ~250x250px).
- Atualize `resume.pdf` com seu currículo real e mantenha o link do botão "Baixar CV" apontando para ele.
- Verifique no `index.html` se o email em `mailto:` está correto (atualmente: `guilherme.fitl10@gmail.com`).
- Adicione screenshots dos projetos na seção `#projects` para melhor apresentação.

---

## Deploy (opções rápidas)

Opção 1 — GitHub Pages (recomendado para sites estáticos):
1. Commit e push do repositório para GitHub.
2. No GitHub, vá em Settings → Pages, escolha a branch `main` (ou `gh-pages`) e a pasta `/ (root)`.
3. Salve; o site ficará disponível em `https://<seu-usuario>.github.io/<repo>`.

Opção 2 — Netlify:
1. Crie conta no Netlify e conecte ao repositório GitHub.
2. Configure um site a partir do repositório, branch `main`.
3. Netlify deploya automaticamente e fornece domínio customizável.

Opção 3 — Vercel:
1. Conecte o repositório ao Vercel.
2. Deploy automático (ideal para projetos estáticos também).

---

## SEO & Social Preview
Recomendo adicionar metas Open Graph e Twitter Card no `<head>` (título, descrição e imagem) para melhor compartilhamento em redes sociais e mensagens diretas.

Exemplo mínimo:
```html
<meta property="og:title" content="Guilherme Fitl — Desenvolvedor Front-End">
<meta property="og:description" content="Desenvolvedor Front-End especializado em Angular e Tailwind. Veja meus projetos e entre em contato.">
<meta property="og:image" content="https://seusite.com/preview.png">
<meta name="twitter:card" content="summary_large_image">
```

---

## Acessibilidade e Performance
- O projeto já incorpora focus states e contraste melhorado; recomendo manter atenção em contraste ao adicionar imagens e texto.
- Para otimizar performance, comprima imagens e prefira SVGs vetoriais quando possível.
- Teste com Lighthouse (Chrome DevTools) e corrija avisos de performance e acessibilidade.

---

## Próximos passos sugeridos
- Adicionar página de projetos detalhados (rota ou páginas separadas) com screenshots e estudos de caso.
- Implementar um backend simples (ex.: Netlify Functions ou Formspree) para envio de formulários sem depender do mailto.
- Internacionalização (i18n) se quiser versão em inglês.

---

## Contato
- Email: guilherme.fitl10@gmail.com
- LinkedIn: https://linkedin.com/in/guilhermefitl/
- GitHub: https://github.com/fitlgui

---

## Licença
Licenciado sob a licença MIT — sinta‑se livre para usar o template e adaptar para seus projetos.

---

Se quiser, eu adapto este README para uma versão em inglês, adiciono badges (build, deploy, license) ou gero um `package.json` e um pequeno script de deploy automatizado. Deseja que eu adicione alguma seção extra (ex.: testes, CI, changelog)?
