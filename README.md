# AUTO 071 - Site institucional

Site estático feito só com **HTML + CSS** (sem JavaScript). Não precisa de servidor nem de instalação: basta abrir `html/index.html` no navegador ou publicar a pasta em qualquer hospedagem.

## Estrutura
```
AUTO-071/
├── html/
│   ├── index.html      Início
│   ├── servicos.html   Serviços detalhados + perguntas frequentes
│   ├── galeria.html    Galeria (imagens ilustrativas)
│   ├── sobre.html      Sobre a AUTO 071
│   ├── contato.html    Endereço, horários e mapa
│   └── 404.html        Página de erro
├── css/
│   ├── index.css       Estilos de index.html
│   ├── servicos.css    Estilos de servicos.html
│   ├── galeria.css     Estilos de galeria.html
│   ├── sobre.css       Estilos de sobre.html
│   ├── contato.css     Estilos de contato.html
│   └── 404.css         Estilos de 404.html
└── img/                Imagens em WebP (leves)
```

Cada página usa o seu próprio CSS (mesmo nome do HTML). A parte que se repete em todas (cores, cabeçalho, rodapé) está copiada dentro de cada arquivo, então ao mudar uma cor ou o cabeçalho é preciso alterar nos 6 arquivos.

## Pendências antes de publicar
1. **Domínio:** em todos os `.html`, troque `https://SEU-DOMINIO.com.br` pelo endereço real (é usado só na prévia de compartilhamento no WhatsApp/Facebook).
2. **Contato:** o site ainda não tem telefone/WhatsApp/Instagram. Quando houver, acrescente em `contato.html`, no bloco "Endereço", e no rodapé de cada página.
3. **Endereço:** acrescente o número do imóvel ou ponto de referência.
4. **Fotos reais:** as imagens atuais são ilustrativas. Troque-as por fotos de trabalhos feitos pela loja (mantenha os mesmos nomes de arquivo) e remova o aviso em `galeria.html` e `servicos.html`.
5. **Página 404:** muitas hospedagens exigem que `404.html` fique na raiz do site. Se a sua exigir, mova o arquivo e ajuste os caminhos (`../css/` e `../img/` viram `css/` e `img/`).

## IDs no lugar de classes
Os elementos são identificados por `id` (não há mais `class`). Um id só pode aparecer uma vez por página, então elementos repetidos têm id numerado (`card-1` a `card-6`, `botao-1`, `botao-2`...). Ao criar um elemento repetido novo, dê o próximo número e acrescente o id na lista de seletores do CSS.

## Como editar
- **Cores:** bloco `:root` no início de cada arquivo `.css`.
- **Horários:** procure `<dl id="horarios">` (está em `index.html` e `contato.html`) e no rodapé de cada página.
- **Nova imagem:** salve em WebP, ~800 px de largura, e informe `width` e `height` na tag `<img>`.
- **Menu no celular:** como não há JavaScript, os links do menu aparecem sempre em linha, abaixo do logo.
