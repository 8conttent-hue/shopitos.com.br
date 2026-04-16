# CLAUDE.md — SHOPITOS

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** SHOPITOS
**Nicho:** Negócios e Empreendedorismo
**Keywords:** O Shopitos e um Blog que esta transformando os conhecimentos e estrategias
**Paleta de cores:** ocean | **Fonte:** outfit

O Shopitos é um Blog que está transformando os conhecimentos e estratégias de negócios em torno de marketing digital, vendas online e ecommerce. Nosso trabalho inclui o pesquisa, conhecimento de causa, produção, e revisão de conteúdos recentes e de alta impacto para nossos leitores. A atuação da empresa baseia-se em garantir a excelência na prestação de conteúdo a empresários e desenvolvedores, maximizando a geração de valor para seus negócios, clientes, colaboradores, acionistas e sociedade. Além do conhecimento gratuito que entregamos, um outro produto é a nossa consultoria personalizada.  Nessa consultoria nós entendemos seu negócio, seja lá qual for ele, e se compreendermos que podemos mudar seu negócio através de novas estratégias, entra em ação a nossa equipe altamente qualificada e dedicada a fazer seu negócio vender mais e melhor. Para saber mais, entre em contato



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-A |
| Hero | Hero-D |
| Features | Features-H |
| About Section | About-E |
| Posts | Posts-D |
| Footer | Footer-J |
| Página Sobre | Sobre-B |
| Página Contato | Contato-E |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
