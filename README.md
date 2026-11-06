# Rumo ao Maraca: Jogo 2D Rubro-Negro

Jogo de plataforma 2D desenvolvido em **HTML, CSS e JavaScript**, com visual rubro-negro, personagens animados, itens colecionáveis, adversários, checkpoints e cinco fases progressivas.

O projeto funciona diretamente no navegador e não exige instalação, servidor ou dependências externas. Todos os sprites e recursos visuais estão incorporados ao próprio arquivo HTML.

## Demonstração

Abra o arquivo `jogo_flamengo_5_fases.html` em um navegador moderno para iniciar o jogo.

## Características

- Cinco fases completas e progressivas
- Personagem com animações de repouso, corrida, salto e queda
- Cenários com efeito de paralaxe
- Plataformas, obstáculos e adversários
- Oito bolas obrigatórias por fase
- Três estrelas opcionais por fase
- Dois checkpoints em cada fase
- Sistema de três vidas
- Cronômetro e indicador de progresso
- Partículas, iluminação e tremor de câmera
- Controles para computador e dispositivos móveis
- Funcionamento offline
- Arquivo único, sem bibliotecas externas

## Fases

1. **Praia Rubro-Negra**
2. **Centro do Rio**
3. **Morro da Nação**
4. **Noite de Libertadores**
5. **Final no Maraca**

As distâncias entre as plataformas foram ajustadas para permitir a conclusão utilizando o salto normal. A corrida com `Shift` ajuda na movimentação, mas não é obrigatória para atravessar os vãos principais.

## Objetivo

Colete as **oito bolas** de cada fase e alcance a entrada do estádio. As estrelas são opcionais e servem como desafio adicional.

Ao chegar ao final sem todas as bolas necessárias, o personagem será impedido de concluir a fase e receberá uma indicação de quantas bolas ainda faltam.

## Controles

| Ação | Teclado |
|---|---|
| Mover para a esquerda | `A` ou `←` |
| Mover para a direita | `D` ou `→` |
| Pular | `W`, `↑` ou `Espaço` |
| Correr | `Shift` |
| Reiniciar a fase | `R` |

Em celulares e tablets, os controles aparecem automaticamente na tela.

## Como executar localmente

### Opção 1: abrir diretamente

1. Baixe ou clone este repositório.
2. Localize o arquivo `jogo_flamengo_5_fases.html`.
3. Abra o arquivo com Google Chrome, Microsoft Edge, Mozilla Firefox ou Safari.

### Opção 2: usar um servidor local

Com Python instalado, execute no diretório do projeto:

```bash
python -m http.server 8000
```

Depois, acesse:

```text
http://localhost:8000/jogo_flamengo_5_fases.html
```

Um servidor local não é obrigatório, mas pode facilitar testes durante o desenvolvimento.

## Publicação no GitHub Pages

1. Crie um repositório no GitHub.
2. Adicione `jogo_flamengo_5_fases.html` e este `README.md`.
3. Renomeie o arquivo do jogo para `index.html` se quiser que o jogo abra diretamente na página principal.
4. No repositório, acesse **Settings > Pages**.
5. Em **Build and deployment**, selecione **Deploy from a branch**.
6. Escolha a branch `main` e a pasta `/ (root)`.
7. Clique em **Save**.

Após a publicação, o GitHub Pages exibirá o endereço público do jogo.

## Estrutura recomendada

```text
rumo-ao-maraca/
├── index.html
├── README.md
├── LICENSE
└── screenshots/
    └── gameplay.png
```

Como os recursos visuais estão incorporados ao HTML, não é necessário manter uma pasta separada de imagens para o jogo funcionar.

## Tecnologias

- HTML5
- CSS3
- JavaScript
- Canvas 2D
- Sprites em PNG incorporados em Base64

## Compatibilidade

O jogo foi projetado para navegadores modernos com suporte a:

- HTML Canvas
- JavaScript ES6
- Pointer Events
- Imagens PNG com transparência

Navegadores recomendados:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Safari

## Desenvolvimento

O jogo utiliza um único arquivo HTML, que contém:

- Estrutura da interface
- Estilos visuais
- Lógica das fases
- Física do personagem
- Detecção de colisões
- Sistema de câmera
- Animações
- Sprites codificados em Base64

Para alterar o jogo, abra o arquivo HTML em um editor como Visual Studio Code e procure pelas seguintes estruturas no JavaScript:

- `themes`: nomes e cores das fases
- `makeLevel()`: geração das plataformas, itens e adversários
- `update()`: física, colisões e regras
- `draw()`: renderização do cenário e personagens
- `F`: coordenadas dos quadros de animação do personagem

## Melhorias futuras

- Música e efeitos sonoros
- Tela de seleção de fases
- Salvamento do progresso no `localStorage`
- Chefes ao final das fases
- Novos tipos de adversários
- Sistema de pontuação total
- Ranking local
- Suporte a controle gamepad
- Modo tela cheia
- Novas animações e cenários

## Aviso sobre marcas

Este é um projeto independente e não oficial, criado para fins de estudo e entretenimento. O projeto não possui vínculo, patrocínio ou aprovação do Clube de Regatas do Flamengo.

Nomes, escudos, símbolos e demais marcas de terceiros pertencem aos respectivos titulares. Antes de distribuir comercialmente ou promover publicamente o projeto, substitua recursos protegidos ou obtenha as autorizações necessárias.

## Licença

O código pode ser disponibilizado sob a licença escolhida pelo proprietário do repositório. Para um projeto aberto e permissivo, uma opção comum é a licença MIT.

Se utilizar a licença MIT, adicione um arquivo `LICENSE` ao repositório e confirme que todos os recursos visuais também podem ser redistribuídos sob os termos escolhidos.

---

Desenvolvido como um jogo de plataforma 2D rubro-negro para navegador.
