# Jogo de Adivinhação

Este é um simples jogo de adivinhação desenvolvido em JavaScript. O jogador precisa adivinhar um número secreto entre 1 e 10.

## Como jogar
1. Clone este repositório.
2. Abra o arquivo `index.html` em seu navegador.
3. Digite um número no campo e clique em "Verificar".



# Explicação Detalhada

Variáveis Globais:

listaDeNumerosSorteados: Um array para armazenar os números já sorteados, evitando repetições.
numeroLimite: Define o intervalo máximo para o número secreto (10 neste caso).
numeroSecreto: Armazena o número aleatório gerado.
tentativas: Conta o número de tentativas do usuário.
Funções:

exibirTextoNaTela(tag, texto):
Busca um elemento HTML com a tag especificada.
Atribui o texto fornecido ao conteúdo do elemento.
Utiliza a biblioteca responsiveVoice para ler o texto em voz alta.
exibirMensagemInicial():
Chama a função exibirTextoNaTela para exibir o título do jogo e as instruções iniciais.
verificarChute():
Obtém o valor do chute do usuário.
Compara o chute com o número secreto.
Exibe mensagens de acerto ou erro, informando se o número secreto é maior ou menor.
Incrementa o contador de tentativas.
Limpa o campo de entrada.
gerarNumeroAleatorio():
Gera um número aleatório entre 1 e numeroLimite.
Verifica se o número já foi sorteado anteriormente.
Se já foi sorteado, chama a função recursivamente até gerar um número único.
Adiciona o número sorteado à lista de números já sorteados.
limparCampo():
Limpa o campo de entrada para o próximo chute.
reiniciarJogo():
Gera um novo número secreto.
Limpa o campo de entrada.
Reinicia o contador de tentativas.
Exibe a mensagem inicial.
Desabilita o botão de reiniciar até que o usuário faça um novo chute.
Fluxo do Jogo:
Inicialização: O código define as variáveis globais e chama a função exibirMensagemInicial para apresentar o jogo ao usuário.
Chute do Usuário: O usuário digita um número e clica em um botão (não mostrado no código) para verificar o chute.
Verificação: A função verificarChute compara o chute com o número secreto e fornece feedback ao usuário.
Reinício: Após acertar o número, o usuário pode clicar no botão de reiniciar para iniciar uma nova partida.
