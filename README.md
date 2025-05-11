Detona Ralph RPG
Um jogo de navegador inspirado no personagem Ralph, que combina elementos de jogos clássicos de arcade com mecânicas modernas de RPG.


Detona Ralph RPG é uma versão aprimorada do clássico jogo "Whack-a-Mole", onde o jogador deve clicar no personagem Ralph quando ele aparece em diferentes janelas. Esta versão adiciona elementos de RPG como sistema de vida, níveis de jogador, habilidades, loja de itens e chefes.

🎮 Funcionalidades
Sistema de Combate: Clique no Ralph para atacá-lo antes que ele ataque você

Progressão de Personagem: Ganhe XP, suba de nível e aumente seu dano

Sistema de Vida: Inimigos causam dano se não forem eliminados a tempo

Combos: Acerte inimigos consecutivamente para multiplicar pontos e XP

Loja de Habilidades: A cada 5 níveis, compre habilidades especiais com pontos

Chefes: Enfrente um chefe poderoso a cada 5 níveis

Power-ups: Colete itens especiais durante o jogo para obter vantagens temporárias

Sistema de Recordes: Salve e visualize suas melhores pontuações

🛠️ Tecnologias Utilizadas
HTML5: Estrutura da página e elementos do jogo

CSS3: Estilização, animações e responsividade

JavaScript: Lógica do jogo e interatividade

LocalStorage API: Armazenamento de recordes

📚 Arquitetura do Código
Estrutura de Arquivos
text
detona-ralph/
├── index.html
├── src/
│   ├── scripts/
│   │   └── engine.js
│   ├── styles/
│   │   ├── reset.css
│   │   └── main.css
│   ├── images/
│   │   ├── ralph.png
│   │   ├── ralph-hit.png
│   │   ├── wall.png
│   │   ├── clock.png
│   │   ├── star.png
│   │   ├── hourglass.png
│   │   ├── heart.png
│   │   └── shield.png
│   └── audios/
│       ├── hit.m4a
│       ├── miss.m4a
│       ├── levelUp.m4a
│       ├── gameOver.m4a
│       ├── playerHit.m4a
│       ├── heal.m4a
│       ├── shield.m4a
│       ├── playerLevelUp.m4a
│       ├── purchase.m4a
│       ├── slowTime.m4a
│       ├── doublePoints.m4a
│       └── extraTime.m4a
Padrões de Design
O jogo utiliza um padrão de design baseado em estado (state pattern) para gerenciar os diferentes aspectos do jogo:

javascript
const state = {
    values: { /* valores do jogo */ },
    view: { /* referências aos elementos do DOM */ },
    actions: { /* timers e ações */ },
    enemies: { /* configurações dos inimigos */ }
};
🎲 Mecânicas de Jogo
Sistema de RPG
Vida do Jogador: Começa com 100 pontos de vida

Níveis de Jogador: Aumenta o dano e recupera vida ao subir de nível

Experiência (XP): Ganhe XP ao derrotar inimigos, com bônus por combos

Tipos de Inimigos
Normal: Dano baixo, poucos pontos e XP

Especial: Dano médio, pontos e XP moderados

Perigoso: Dano alto, bons pontos e XP

Chefe: Dano muito alto, muitos pontos e XP

Power-ups
Tempo Lento: Reduz a velocidade do jogo

Pontos Dobrados: Dobra os pontos por acerto

Tempo Extra: Adiciona 10 segundos

Cura: Recupera parte da vida

Escudo: Protege contra o próximo ataque

Loja de Habilidades
Abre automaticamente a cada 5 níveis, oferecendo itens como:

Escudo Extra: Bloqueia dois ataques inimigos

Cura Rápida: Recupera 50% da vida instantaneamente

Dano Crítico: Chance de causar dano crítico dobrado

Aumento de Dano: Aumenta seu dano em 20%

XP Bônus: Ganha 20% mais XP por inimigo derrotado

🚀 Como Executar
Clone o repositório:

bash
git clone https://github.com/seu-usuario/detona-ralph.git
Navegue até a pasta do projeto:

bash
cd detona-ralph
Abra o arquivo index.html em um navegador web moderno

Alternativamente, você pode usar a extensão "Live Server" do VS Code para executar o projeto.

🧠 Conceitos Técnicos Aplicados
Event Listeners: Para capturar cliques do usuário

Timers e Intervals: Para controlar o tempo e a aparição dos inimigos

DOM Manipulation: Para atualizar a interface do jogo

CSS Animations: Para feedback visual e efeitos

LocalStorage: Para persistência de dados (recordes)

Responsive Design: Adaptação para diferentes tamanhos de tela

State Management: Gerenciamento de estado do jogo

Object-Oriented Programming: Organização do código em objetos e métodos

🎯 Desafios e Soluções
Pausa do Jogo: Implementação de um sistema de pausa que interrompe todos os timers quando a loja é aberta ou um chefe aparece

Chefes: Criação de um sistema de chefes com mecânicas próprias e recompensas especiais

Balanceamento: Ajuste cuidadoso dos valores de dano, XP e pontos para garantir progressão satisfatória

📝 Possíveis Melhorias
Adicionar mais tipos de inimigos

Implementar um sistema de habilidades ativas com cooldown

Criar diferentes fases com cenários distintos

Adicionar efeitos sonoros mais variados

Implementar um sistema de conquistas

📜 Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

👨‍💻 Autor
Desenvolvido como parte de um projeto educacional para demonstrar conceitos modernos de desenvolvimento de jogos web.

