# MeuPrimeiroProjeto
O que é? 
Este é um simples jogo de Pedra, Papel, Tesoura que você joga contra o computador. O jogo faz escolhas aleatorias entre Pedra, Papel e Tesousa, e o usuário deve tentar vencê-lo.

Como funciona o jogo Pedra, Papel e Tesoura?
Regras básicas: 
- O usuario é solicitado a escolher entre "pedra", "papel", e "tesoura"
- O computador também vai escolher aleatoriamente uma dessas opções.
- As regras  do jogo são:
- Pedra vence tesoura
- Papel vence pedras
- Tesoura vence papel
- Se ambos escolherem a mesma opção, é empate.

Como construir o jogo?
-Certifique-se de ter o .NET instalado
-Para executar o projeto, use os seguintes comandos:
string[] opcoes =
Random random = new Random();
while (true)
string jogador = Console.ReadLine().ToLower();
string computador = opcoes[random.Next(opcoes.Length)];
Console.WriteLine($"O computador escolheu: {computador}");
else if (jogador == "pedra" && computador == "tesoura" || jogador == "papel" && computador == "pedra" || jogador == "tesoura" && computador == "papel")