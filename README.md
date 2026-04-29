# ⚽ CopaNaMão — Protótipo de Baixa Fidelidade

> Atividade Prática de Prototipagem | Disciplina: IHC & UX  
> Ferramenta utilizada: Miro (Wireframe Low-Fidelity)

---

## 👥 Integrante

Nome: Herbert Silva de Freitas
RA: 4261212304


---

##  Problema Focado

A FIFA identificou três grandes dores dos torcedores dentro dos estádios durante a Copa do Mundo. Entre elas, **priorizamos resolver duas principais**:

### 1. Filas imensas nos quiosques de comida
O torcedor precisa abandonar o seu assento, enfrentar filas longas em ambientes lotados e barulhentos, e frequentemente perde lances importantes do jogo enquanto espera. Em um evento como a Copa do Mundo, onde cada segundo em campo tem valor emocional altíssimo, esse atrito gera frustração direta.

### 2. Perda de lances importantes durante ausências do assento
Mesmo quando o torcedor precisa se ausentar por qualquer motivo (banheiro, comida, portão), ele fica sem acesso aos momentos decisivos da partida. Não existe hoje, dentro do estádio, uma forma rápida e oficial de rever um lance polêmico ou um gol de múltiplos ângulos em tempo real.

**Dor central priorizada:** o torcedor não consegue aproveitar 100% da experiência dentro do estádio porque qualquer deslocamento representa perda de jogo, e não há ferramenta que compense essa ausência.

---

##  Justificativa de Design

### Hierarquia da Informação
A tela inicial (Home/Dashboard) foi projetada com o placar ao vivo no topo e em destaque, pois é a informação que o torcedor consulta primeiro ao pegar o celular. Abaixo do placar, os quatro atalhos rápidos — Mapa, Comida, Replay e Stats — foram dispostos em grade 2×2 com botões grandes, priorizando o uso em ambiente de alta distração (barulho, escuridão, adrenalina).

### Botões Grandes e Leitura Clara
Todos os botões de ação primária ocupam pelo menos 38px de altura e apresentam rótulo textual simples, sem depender de ícones ambíguos. A decisão segue o princípio de affordance em contexto de pressão: o torcedor está com atenção dividida entre o celular e o campo, portanto os alvos de toque precisam ser generosos e autoexplicativos.

### Navegação pelo Bottom Navigation Bar
A barra de navegação inferior fixa com quatro destinos (Home, Mapa, Comida, Replay) garante que o usuário nunca precise mais do que um toque para acessar qualquer funcionalidade principal. Isso reduz a carga cognitiva e elimina a necessidade de memorizar caminhos de navegação.

### Fluxo de Pedido Dentro do Contexto
O cardápio foi posicionado atrás de um único atalho da tela inicial. A opção de entrega no assento é marcada como padrão na tela de carrinho, pois é o caminho que mantém o torcedor no lugar — reforçando a solução central do problema. A escolha consciente de retirar no quiosque fica como opção secundária.

### Replay Acessível e Contextualizado
A tela de Replay apresenta primeiro o lance mais recente em destaque (player grande), com seletor de ângulos logo abaixo, seguido de uma lista cronológica dos lances anteriores. Essa organização reduz o tempo de busca: o torcedor que acabou de perder um gol encontra o replay em menos de dois toques.

### Identidade Visual de Baixa Fidelidade
O protótipo foi construído intencionalmente em preto, branco e cinza, sem cores, imagens reais ou detalhes visuais finais. Isso mantém o foco da avaliação na estrutura, no fluxo e na usabilidade, evitando que decisões estéticas influenciem o feedback nesta fase.

---

##  Fluxo do Usuário

### 🍔 Fluxo 1: Pedir um Lanche

[Tela 1 — Home]
O torcedor está no assento.
Vê o atalho [Comida] na grade de acesso rápido.
→ Toca em [Comida]

[Tela 3 — Cardápio Digital]
Visualiza os itens disponíveis para o seu setor (Setor B4).
Navega pelas abas: Lanches | Bebidas | Doces | Combos.
Encontra "Hot Dog Copa" e toca em [+ Add].
Adiciona também "Coca-Cola 500ml".
→ Toca no botão "Ver Carrinho (2 itens) →"

[Tela 4 — Carrinho / Pagamento]
Confirma os itens e os preços.
Verifica que a opção [✓] Entregar no assento B4 — Fila 12 — Assento 07
já está selecionada por padrão.
Seleciona a forma de pagamento: [Cartão].
→ Toca em "CONFIRMAR PEDIDO | R$ 98,00"

[Tela 1 — Home, após confirmação]
Uma notificação aparece na Home:
"[!] Pedido #42 pronto! Retire no Quiosque 7"
(caso tenha escolhido retirada)
— ou —
O pedido chega diretamente ao assento.
O torcedor não saiu do lugar e não perdeu nenhum lance.

---

### ▶️ Fluxo 2: Ver um Replay

[Tela 1 — Home]
Ocorre um gol polêmico enquanto o torcedor estava olando o celular.
Vê o atalho [Replay] na grade de acesso rápido.
→ Toca em [Replay]

[Tela 5 — Central de Replays]
A tela abre diretamente no lance mais recente em destaque:
"GOL! Neymar Jr. — 66'"
O player de vídeo já está carregado com o ângulo principal.
→ Toca em [> PLAY]

Quer ver o lance de outro ângulo?
→ Toca em [VAR] ou [Câm. Gol] ou [Aérea]
O vídeo recarrega com o novo ângulo.

Quer ver um lance anterior?
→ Rola a lista "Lances Recentes" abaixo do player.
Encontra "GOL Argentina — Messi | 45'"
→ Toca em "Assistir →"
O player atualiza com o lance selecionado.

[Retorno à Home]
→ Toca em [Home] na barra de navegação inferior.
Volta ao placar ao vivo sem perder o contexto do jogo.

---

## 🖼️ Telas do Protótipo

| # | Tela | Descrição |
|---|------|-----------|
| 1 | Home / Dashboard | Placar ao vivo, acesso rápido, notificações |
| 2 | Mapa do Estádio | Localização GPS, pontos de interesse, rotas |
| 3 | Cardápio Digital | Itens por setor, abas por categoria |
| 4 | Carrinho / Pagamento | Resumo do pedido, entrega no assento, pagamento |
| 5 | Central de Replays | Player multicâmera, lista de lances recentes |
| 6 | Perfil / Ingresso | QR Code do ingresso, dados do setor, ajuda |

---

## 🛠️ Ferramenta

- **Miro** — Board de prototipagem colaborativa
- Estilo: wireframe de baixa fidelidade (preto, branco e cinza)

---

