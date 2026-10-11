# Circulação Sanguínea em Realidade Aumentada

Protótipo educativo de **realidade aumentada (RA)** desenvolvido para a atividade prática da disciplina *Realidade Virtual e Aumentada*, da UNINTER.

## Objetivo

Visualizar um segmento estilizado de vaso sanguíneo em 3D e observar hemácias se movimentando pelo seu interior, utilizando a câmera de um celular e um marcador de realidade aumentada.

## Funcionalidades

- Visualização de um vaso sanguíneo 3D semitransparente em corte.
- Hemácias bicôncavas animadas para representar o fluxo sanguíneo.
- Detecção do marcador **Hiro** pela câmera do celular.
- Painel educativo adaptado a telas de smartphones.
- Aviso na tela quando o marcador é encontrado ou perdido.

> **Observação:** é uma representação didática, não uma simulação fisiológica nem um modelo em escala anatômica real.

## Tecnologias utilizadas

- HTML5, CSS3 e JavaScript.
- [A-Frame](https://aframe.io/) para renderização 3D.
- [AR.js](https://github.com/AR-js-org/AR.js) para realidade aumentada baseada em marcador.
- [Three.js](https://threejs.org/) por meio do A-Frame para criação das geometrias 3D.
- GitHub Pages para hospedagem estática.

## Estrutura do repositório

```text
hemacia_RA/
├── index.html
└── README.md
```

## Publicação pelo GitHub Pages

1. Crie um repositório **público** no GitHub.
2. Adicione `index.html` e `README.md` na raiz do repositório.
3. Vá em **Settings > Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha a branch `main` e a pasta `/ (root)`; depois salve.
6. Espere o GitHub Pages disponibilizar o endereço HTTPS.

Exemplo de endereço:

`https://SEU-USUARIO.github.io/hemacia_RA/`

## Como executar no celular

1. No notebook ou em uma folha impressa, abra o [marcador Hiro original](https://raw.githubusercontent.com/AR-js-org/AR.js/master/data/images/hiro.png).
2. No celular, abra o site publicado no GitHub Pages usando um navegador com acesso à câmera.
3. Autorize o uso da câmera quando solicitado.
4. Aponte para o marcador Hiro completo, com boa iluminação.
5. Observe o vaso e as hemácias em movimento. Mova o celular lentamente para vê-los de outros ângulos.

**Importante:** é necessária uma conexão com a internet para carregar as bibliotecas externas. O navegador e o aparelho precisam oferecer suporte à câmera e ao WebGL. O marcador físico continuará visível na imagem da câmera fora da região ocupada pelo modelo 3D.

## Como ajustar o tamanho do modelo

No `index.html`, procure:

```html
scale="0.40 0.40 0.40"
```

Para reduzir ainda mais, substitua por:

```html
scale="0.30 0.30 0.30"
```

A distância entre câmera e marcador também influencia o tamanho aparente do modelo.

## Como apresentar o trabalho

1. Apresente o nome e o objetivo do projeto.
2. Mostre o site aberto no celular e autorize o uso da câmera.
3. Aponte para o marcador e demonstre as hemácias em movimento.
4. Explique a função das hemácias no transporte de oxigênio.
5. Explique que a realidade aumentada pode apoiar a educação em biologia e saúde.
6. Grave a tela do celular com sua própria demonstração e explicação.
7. Publique o vídeo no YouTube, preferencialmente como **Não listado**, e entregue o link no AVA UNIVIRTUS.

O documento de orientação da atividade informa que **o projeto funcionando vale 40%**, **sua utilidade vale 30%** e **a qualidade da explicação no vídeo vale 30%**. A publicação no YouTube e a autoria própria também são obrigatórias.

## Autoria e créditos

Projeto acadêmico desenvolvido por Mariana Rodrigues Pius.

Bibliotecas externas: A-Frame e AR.js. O projeto utiliza seus recursos para construir a cena de realidade aumentada; as bibliotecas não foram criadas pela autora.

## Estado atual

Código preparado para publicação e teste. O funcionamento final precisa ser validado em um celular real antes da entrega.
