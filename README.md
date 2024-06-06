# Jogo da Velha com IA em C++

Este é um jogo da velha (tic-tac-toe) implementado em C++ que permite que um jogador humano jogue contra uma IA utilizando o algoritmo Minimax.

## Descrição

O jogo é jogado em um tabuleiro 3x3. Dois jogadores alternam as jogadas colocando seus marcadores (`X` para o jogador humano e `O` para a máquina) em uma célula vazia do tabuleiro. O objetivo é ser o primeiro a formar uma linha de três marcadores na horizontal, vertical ou diagonal.

### Funcionalidades

- O tabuleiro é desenhado de maneira clara e organizada.
- O primeiro jogador é escolhido aleatoriamente (jogador humano ou IA).
- A IA usa o algoritmo Minimax para determinar a melhor jogada possível.
- A tela é limpa a cada jogada para melhorar a visualização.

## Como Jogar

1. Clone o repositório:
    ```sh
    git clone https://github.com/seu-usuario/jogo-da-velha-cpp.git
    cd jogo-da-velha-cpp
    ```

2. Compile o código:
    ```sh
    g++ -o jogo-da-velha main.cpp
    ```

3. Execute o jogo:
    ```sh
    ./jogo-da-velha
    ```

4. Siga as instruções na tela. O tabuleiro é numerado de 1 a 9 conforme o esquema abaixo:
    ```
        1    |      2    |     3     
      (1,1)  |    (1,2)  |   (1,3)  
    ---------|-----------|-----------
        4    |     5     |     6     
      (2,1)  |   (2,2)   |   (2,3)  
    ---------|-----------|-----------
        7    |     8     |     9     
      (3,1)  |   (3,2)   |   (3,3)  
    ```

5. Digite o número correspondente à posição onde deseja colocar seu marcador.

## Estrutura do Código

- `main.cpp`: Contém a implementação do jogo da velha com IA.

### Principais Funções

- `void DrawBoards(std::string play[])`: Desenha o tabuleiro.
- `bool isMovesLeft(std::string board[9])`: Verifica se ainda há movimentos disponíveis.
- `int evaluate(std::string board[9])`: Avalia o tabuleiro para determinar se há um vencedor.
- `int minimax(std::string board[9], int depth, bool isMax)`: Implementa o algoritmo Minimax.
- `int machine(std::string board[9])`: Determina a melhor jogada para a IA.
- `int MovePlayer(std::string board[9])`: Permite ao jogador humano fazer uma jogada.

## Requisitos

- Compilador C++ (como g++)
- Sistema operacional compatível com comandos de limpeza de tela (Windows, Linux, macOS)

## Contribuição

Se você encontrar algum problema ou tiver sugestões de melhorias, sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

