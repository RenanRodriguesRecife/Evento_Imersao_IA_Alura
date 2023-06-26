# Imersao_IA_Alura

- Ele alega que a AI não vai roubar seu emprego mas que alguém que sabe dominar as ferramentas de AI vai.

LLM - ferramentas de IA que geram textos

Ferramentas de LLM (2023):

- ChatGPT

- POE.com (ela dá acesso a vários bots diferentes inclusive o chatGPT)

- Claude (ANTROPIC)

- Modo chat do navegador Bing (chatGPT 4)
    (Por enquanto o Bing é o único que serviço de geração de imagem imbutido da openAI(dolly))

- Bard (precisa de uma VPN - tem como usar o a VPN do opera)

OBS: Os modelos entendem melhor os promts em inglês que em português. 

OBS: O GPT não deve ser visto como um oráculo ele erra (ele procura responder com convicção mesmo estando errado). Os dados do gpt estão atualizados até 2021


OBS: Você pode pedir para o GPT escrever:  "Me diga como seria a pronuncia da primeira frase acima em japônes mas usando uma forma de ler em português"

- Janela de conversa: é quanto tempo você consegue conversar com essas ferramentas de forma com que ele não se perda com o que você estava falando lá trás.

Os modelos LLM não aprendeou os textos e sim como os seres humanos consegue escrever textos. Ele para a próxima palava ele calcula estatiscamente qual seria a próxima palavra viável.

OBS: O chatgpt não consegue nem se quisese gerar a mesma resposta com o mesmo promt. Se você pedir dados no chatgpt ele tem uma grande probabilidade de te dar números aleatórios.

OBS: É importante que você limpe a tela quando for trocar de assunto

Você deve usar o resultado de uma AI como promt em outra ai
EX: 
promt1: Descreva em texto um poster de um jogo Half life 2 episode 3:
promt2: Agora eu quero que você separe o texto em palavras chaves, sem descrição detalhada apenas palavras chaves.

agora você pode usar no midjorney.



AULA 02

Como resumir conteúdos:

Análise de sentimentos:
- Diga qual é o sentimento: Positivo, negativo ou neutro: "cole o texto que você quer analizar"

OBS: Você pode separar os textos colocando um "-" hífen antes dos parágrafos 

```
- Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vel metus sit amet magna lobortis aliquet. Phasellus aliquam orci est, vitae consequat ligula fringilla a. Suspendisse id nulla blandit, aliquet odio ut, dictum mauris. Nam scelerisque tempus quam. In hac habitasse platea dictumst. Nullam diam enim, bibendum euismod mattis vestibulum, dignissim in diam. Phasellus gravida malesuada elementum. Sed vulputate elit lorem, et finibus purus feugiat vitae.

- Mauris sit amet lectus nec arcu egestas feugiat. Vivamus a fringilla elit, ut dictum nulla. Praesent ut neque dictum, auctor enim a, pharetra nunc. In consectetur commodo ligula, in gravida metus gravida at. Morbi mauris massa, sagittis ac commodo sed, laoreet eget ipsum. Ut ornare ultrices aliquet. Phasellus id tortor et justo ullamcorper pharetra. Praesent dapibus vitae ligula at vulputate. Integer tellus nunc, vestibulum in dolor quis, posuere vestibulum quam. Aliquam erat volutpat. Curabitur in lacus leo. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Vivamus quis lectus est. Nullam nunc ex, imperdiet a ex non, rutrum cursus neque.

- Praesent eu orci fringilla, varius quam vitae, aliquet turpis. Proin ullamcorper odio vel interdum euismod. Mauris porta dictum massa at tristique. Aenean id felis nec eros convallis venenatis in imperdiet urna. Proin at tortor interdum, fringilla odio semper, volutpat nulla. Ut mollis arcu vitae justo consequat consequat. Pellentesque sit amet neque nibh. Fusce lectus purus, congue at urna quis, consequat pulvinar ante. Cras id finibus sapien, quis consectetur dolor. Ut finibus lorem in nulla posuere faucibus. Nulla quam magna, porta nec nunc sit amet, gravida fermentum quam. Cras in mauris augue. Aenean eget blandit nisi. Nunc porttitor libero at tellus pellentesque accumsan. Proin fringilla in nisi et ornare. Mauris eget ultrices velit, et sagittis odio.

```
você pode podir para que seja curto e tabelado



Regras:
- seja claro 

- dê o máximo de informações. Ex: se você passar um número diga o que esse número significa: se ele maior é possitivo e menor é negativo...

OBS: 
Ex: Você tem 20 reviews de filmes. E você quer o ChatGPT baseado no review suponha a nota que seria dado pelo crítico.
Como você tá passando várias informações dispersas uma hora o chat vai se perder e misturar as coisas. Para ter mais precisão é ideal você separar cada um por um promt.



OBS: O chatgpt não é bom em matemática. Um dia o chatGPT vai erra quanto é 4 + 4.

OBS: Sempre coloque o exemplo do formato da saída no início do promt. Evite colar no final.


OBS: Evite usar o ChatGPT para fazer funções que outras ferramentas já são muito bom para isso: Ex: Converter JSON para CSV.



Integrações (Usando API):

Integrar Google SpriteSheets com o ChatGPT: Nas extenções tem o ADDON(complementos) SheetGPT (2023)

=GPT("o promt que você quer executar")

A avaliação que o promt faz com um elemento é muito mais exato que a avaliação que ele faz com 20 elementos de uma vez.



Ex:

´´´
=GPT("Qual a nota de 0 a 10 que a pessoa daria para a o filme com a seguinte avaliação: "&C1)


=GPTLIST -> ele gera um resultado para cada célula em uma lista

=GTPIMAGE -> cria uma imágem

Framer.AI -> pode gerar um site

---------------------------------
Aula 03 - Engenharia de Promt


