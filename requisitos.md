# Requisitos funcionais e não funcionais do jogo "Ribeirão Noir: O Roubo da Estátua de São Sebastião"

## Sumário

- [Requisitos funcionais](#requisitos-funcionais)
  - 1.  Sistema de Rolagem de Dados
  - 2.  Navegação e Interface Principal
  - 3.  Sistema de Personagens e Profissões
  - 4.  Sistema de Localizações
  - 5.  Sistema de Pistas e Investigação
  - 6.  Sistema de Narrativa e Escolhas
  - 7.  Sistema de Salvamento
  - 8.  Sistema de Configurações
- [Requisitos não funcionais](#requisitos-não-funcionais)
  - 1.  Acessibilidade
  - 2.  Portabilidade
  - 3.  Segurança
  - 4.  Manutenibilidade
  - 5.  Usabilidade e Localização

## Requisitos funcionais

### 1. Sistema de Rolagem de Dados

- **RF01:** Como jogador, quero que ao solicitar rolagem, a animação seja exibida sobre a interface de jogo e, ao final, retorne automaticamente à cena de jogo.
- **RF02:** Como jogador, quero um botão "Rolar Dados Novamente" que só aparece se eu tiver mais de 1 PV, para poder tentar novamente gastando pontos de vida.
- **RF03:** Como jogador, quero que ao rolar novamente, 1 PV seja subtraído antes de reexibir a animação.
- **RF04:** Como jogador, quero aguardar a conclusão completa da animação de rolagem antes de ver o resultado numérico.
- **RF05:** Como jogador, quero somar habilidades e itens ao resultado da rolagem para aumentar minhas chances de sucesso.

### 2. Navegação e Interface Principal

- **RF06:** Como jogador, quero uma barra fixa inferior com botões de acesso rápido: "Informações da personagem", "Pistas", "Conquistas", "Configurações", "Personagens" e "PV (Pontos de vida)".
- **RF07:** Como jogador, quero que o botão "Continuar Jogo" apareça na tela inicial somente se existir um estado salvo de partida.
- **RF08:** Como jogador, quero acessar a tela principal do escritório com botões para "Mapa", "Pistas" e "Solucionar Mistério".

### 3. Sistema de Personagens e Profissões

- **RF09:** Como jogador, quero escolher ao iniciar uma das três profissões (advogada, jornalista ou investigadora particular), para que cada personagem apresente atributos e diálogos diferenciados.
- **RF10:** Como jogador, quero uma tela de perfil ("Dandara") que exiba nome, profissão, comportamentos, medalhas e conquistas.

### 4. Sistema de Localizações

- **RF11:** Como jogador, quero visualizar uma tela interativa com os 11 marcos históricos de Ribeirão Preto para selecionar locais de investigação.
- **RF12:** Como jogador, quero ver a descrição contextual de cada local ao selecioná-lo, antes de ingressar na cena.

### 5. Sistema de Pistas e Investigação

- **RF13:** Como jogador, quero uma tela "Pistas" que liste cada pista coletada com título e descrição detalhada.
- **RF14:** Como jogador, quero uma tela "Pessoas" que liste personagens investigados, incluindo nome e descrição.
- **RF15:** Como jogador, quero coletar pistas ao avançar no jogo e acompanhar meu progresso investigativo.

### 6. Sistema de Narrativa e Escolhas

- **RF16:** Como jogador, quero que cada cena apresente contexto narrativo e múltiplas opções de escolha que direcionam o enredo de forma não-linear.
- **RF17:** Como jogador, quero acessar "Solucionar Mistério" ao reunir pistas suficientes e escolher um acusado dentre os personagens.

### 7. Sistema de Salvamento

- **RF18:** Como jogador, quero que o sistema salve automaticamente todo o texto da cena atual e variáveis de progresso ao sair do jogo.
- **RF19:** Como jogador, quero retomar de onde parei quando clicar em "Continuar Jogo".

### 8. Sistema de Configurações

- **RF20:** Como jogador, quero uma tela de "Configurações" para ajustar volume de música e efeitos, ativar/desativar legendas.

---

## Requisitos não funcionais

### 1. Acessibilidade

- **RNF01:** A interface deve atender ao nível AA da WCAG com contraste mínimo 4.5:1.
- **RNF02:** Suporte a ajustes de tamanho de fonte.
- **RNF03:** Legendas para diálogos e audiodescrição de conteúdos sonoros.

### 2. Portabilidade

- **RNF04:** Framework para disponibilidade em Android (min. 8.0).
- **RNF05:** Pacote de instalação inferior a 100 MB para facilitar download em rede móvel.

### 3. Segurança

- **RNF06:** Comunicações para updates via HTTPS com certificado válido.
- **RNF07:** Nenhum dado sensível exposto em texto puro no dispositivo.

### 4. Manutenibilidade

- **RNF08:** Lógica de narrativa ramificada modularizada em arquivos de cena independentes.
- **RNF09:** Componentes de UI (botões, barras, listas) modularizados para fácil reconfiguração de cores e layout via temas.
- **RNF10:** Lógica de rolagem e decremento de PV desacoplada do motor de cenas para futura extensão.

### 5. Usabilidade e Localização

- **RNF11:** Textos e diálogos em linguagem clara e simples, revisados por consultoria pedagógica.
- **RNF12:** Interface totalmente traduzida para português brasileiro, com opção para futuras localizações.
