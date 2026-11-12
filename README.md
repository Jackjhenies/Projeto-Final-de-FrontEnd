# AUTO 071 — Estética Automotiva

**Site institucional da AUTO 071, estética automotiva em Jacaraú, Paraíba.**

## Sobre o projeto

Site estático e multipágina criado para apresentar a **AUTO 071**: os serviços oferecidos, a galeria de trabalhos, a história do negócio, além de endereço, horários de funcionamento e mapa de localização.

O foco do projeto é ser **leve, rápido e acessível**, usando apenas HTML e CSS puros, sem frameworks, sem JavaScript e sem etapa de build.

## Páginas

| Página | Arquivo | Descrição |
| --- | --- | --- |
| Início | `html/index.html` | Apresentação, resumo dos serviços, chamada para visita e horários |
| Serviços | `html/servicos.html` | Detalhamento dos seis serviços oferecidos |
| Galeria | `html/galeria.html` | Imagens dos serviços realizados |
| Sobre | `html/sobre.html` | Quem somos e a identidade da marca |
| Contato | `html/contato.html` | Endereço, horários, rota no Google Maps e mapa incorporado |
| Erro 404 | `html/404.html` | Página personalizada para endereços não encontrados |

## Serviços apresentados

- Lavagem detalhada
- Higienização interna
- Polimento
- Vitrificação
- Enceramento
- Restauração de faróis

## Destaques técnicos

- **HTML semântico**: uso de `header`, `nav`, `main`, `section`, `footer`, `address` e `dl`.
- **Acessibilidade**: link "pular para o conteúdo", `aria-label` na navegação, `aria-current` na página ativa, textos alternativos descritivos nas imagens e título no `iframe` do mapa.
- **Responsividade**: layout adaptado a telas de celular, tablet e desktop por meio de *media queries*.
- **Preferência de movimento reduzido**: respeita `prefers-reduced-motion`.
- **Desempenho**: imagens em formato **WebP**, `loading="lazy"` nas imagens abaixo da dobra, `width` e `height` definidos para evitar saltos de layout e `preload` da imagem principal.
- **Identidade visual**: paleta em preto, grafite e dourado, definida com variáveis CSS e fonte do sistema (`Segoe UI`, `Roboto`, `Helvetica Neue`, `Arial`), sem dependência de fontes externas.

## Tecnologias

- HTML5
- CSS3 (variáveis CSS, Flexbox/Grid e *media queries*)
- Google Maps (incorporação por `iframe` e link de rota)

## Estrutura de pastas

```text
AUTO-071/
├── css/
│   ├── index.css
│   ├── servicos.css
│   ├── galeria.css
│   ├── sobre.css
│   ├── contato.css
│   └── 404.css
├── html/
│   ├── index.html
│   ├── servicos.html
│   ├── galeria.html
│   ├── sobre.html
│   ├── contato.html
│   └── 404.html
├── img/
│   ├── servicos/
│   │   ├── lavagem-detalhada.webp
│   │   ├── higienizacao-interna.webp
│   │   ├── polimento.webp
│   │   ├── vitrificacao.webp
│   │   ├── enceramento.webp
│   │   └── restauracao-farois.webp
│   ├── hero-polimento.webp
│   ├── logo-auto-071.webp
│   ├── logo-selo.webp
│   └── og-image.jpg
└── README.md
```

Cada página HTML carrega a sua própria folha de estilo, o que mantém o CSS de cada tela enxuto e independente.

## Como executar localmente

Não há instalação nem dependências. Basta ter um navegador moderno.

**1. Clone o repositório**

```bash
git clone <URL-DO-REPOSITORIO>
cd AUTO-071
```

**2. Abra o site**

Abra o arquivo `html/index.html` diretamente no navegador.

**Opcional: servidor local**

Para simular melhor um ambiente de hospedagem, sirva a pasta com qualquer servidor estático:

```bash
# Python
python -m http.server 8000

# ou Node.js
npx serve .
```

Depois acesse `http://localhost:8000/html/index.html`.

## Publicação

Por ser um site estático, eu subi ele para o VERCEL para um acesso mais facil.

- Link para o site:`https://auto-071-9wzsjggrj-jackjhenies-igor-rafael.vercel.app`.


## Informações do negócio

| | |
| --- | --- |
| **Endereço** | Rua Presidente João Pessoa, Jacaraú - PB |
| **Segunda a sexta** | 08:00 às 17:00 |
| **Sábado** | 08:00 às 12:00 |
| **Domingo** | Fechado |

## Licença e direitos

© 2026 AUTO 071 Estética Automotiva. Todos os direitos reservados.

O código, o texto, o logotipo e as imagens deste repositório pertencem à AUTO 071. Não é permitido reproduzir ou redistribuir o material sem autorização.