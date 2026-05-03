# Gerador de Senhas Wi-Fi PT-BR

Página simples para criar uma senha forte para o Wi-Fi, visualizar um QR Code e baixar um PNG com os dados da rede.

## O que este projeto faz

- gera senhas no estilo passphrase com palavras em português
- permite ajustar a quantidade de palavras e incluir números ou caractere especial
- cria um QR Code para facilitar a conexão na rede
- exporta um PNG com QR Code, nome da rede, senha e data

## Segurança da senha

Este projeto usa uma abordagem inspirada em Diceware, adaptada para português. Em vez de depender de uma senha curta e difícil de lembrar, ele monta passphrases com palavras reais escolhidas aleatoriamente a partir de uma lista local.

Na prática, isso ajuda a equilibrar segurança e uso no dia a dia:

- 4 palavras oferecem um nível inicial de proteção com leitura mais fácil
- 5 ou 6 palavras aumentam bastante a resistência contra tentativas de adivinhação
- números e caractere especial podem acrescentar uma camada extra de variação

Cada palavra vem de uma lista com milhares de opções. Isso aumenta a entropia da senha, ou seja, a quantidade de combinações possíveis. Quanto mais palavras aleatórias, mais difícil fica prever ou forçar a combinação correta.

## Como usar

1. Abra o arquivo `index.html` no navegador.
2. Digite o nome da sua rede Wi-Fi.
3. Escolha o formato da senha.
4. Clique em **Gerar senha**.
5. Copie a senha ou baixe o QR Code em PNG.

## O que aparece no resultado

- senha gerada na tela
- QR Code da rede Wi-Fi
- nome da rede
- data de geração
- opção para baixar tudo em PNG

## Limitações conhecidas

- o QR exportado usa o formato `WIFI:T:WPA;...`, adequado para o fluxo atual de redes com senha
- a compatibilidade final do QR depende do leitor do celular e da configuração da rede
- o ideal é testar o QR gerado em um aparelho real antes de imprimir ou compartilhar
- o projeto foi pensado para uso direto no navegador, sem backend e sem internet
