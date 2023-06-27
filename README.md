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

Expansão de texto
Resumo de Texto
transformações (tradução, correção)
Classificação

prompt: Vamos simular como funciona o ChatGPT, para cada frase que eu escrever no prompt, você deve listar as 5 palavras com maior probabilidade que você usaria para completá-la, junto com a probabilidade de cada uma delas. Apenas as palavras e probabilidade, sem mais nada. Entendeu?

prompt:  A capital do Brasil é

```

1. Brasilia - 0.95
2. Rio de Janeiro - 0.03
3. São paulo - 0.02
4. Belo Horizonte - 0.01
5. Salvador - 0.01

```

O GPT não faz conta ele calcula probabilidades
O gpt não pega a palavra que tem a maior probabilidade as vezes ele pega a 2 ou 3 terceira para dar um tom mais humano


Você pode pegar um artigo difícil de entender. E pedir para chatGPT escrever como se estivesse escrevendo para uma criança de 10 anos.

Ele pode naõ acertar. Mas ele escreve texto que fazem sentido mas pode não está correto.


Boas práticas:

Escrever instruções de forma clara

Expansão de texto:

Expessificar, dando o máximo de informação que você pode:

Sobre a imersão:
A imersão são 5 aulas que abordam AI generativas com ChatGPT, Bing, Veremos integração com Google SHeets, uso de plugin do GPT. Engenharia de prompt. Os professores da imersão são Paulo, Guilherme, Sérgio. O público alvo é pessoas iniciantes de deversas áreas interessadas em aplicar IA.

Dizer quantos paragravos você quer que o texto tenha:
Siga as regras para criar o post:
Ex: 
- Um post possui 4 parágrafos.
- 5 hashtags em maiuscula.
- Use emojis em todos os parágrafos.
- O texto deve ser épico gerando um storytelling como a jornada do heroi

O link para inscrição é alura.com.br/imersão-ia

GPT4 - consegue intepretar melhor as ordem ambíguas


Se você tem tarefas complexas deve ser subdividadas em tarefas menores mais claras.

O prompt: O texto deve ser épico gerando um storytelling como a jornada do heroi

pode ser quebrado em :
O texto deve ser épico gerando um storytelling como a jornada do heroi:
- Comece com uma pessoa iniciante
- essa pessoa tem um problema no mundo real
- ela passa por dificuldades mas consegue atingir seu objetivo com a juda da inteligência artificial


Regras deve ser claras
Regras complexas devem ser transformadas em regras simples
Deve ser enumeradas
Deve ser explicitas
E dar exemplos

Você pode dar exemplos de textos para ela seguir.
Quando você dá um prompt sem exemplo é considerado 0 shot

quando você coloca um texto de exemplo: 1 shot
FFW shots - dar vários exemplos

Você deve dár vários exemplos para cobrir as possibilidades
Ex:
fassa tal coisa seguindo o exemplo do texto a seguir:


CHAIN OF THOUGHT (CADEIA DE PENSAMENTO) - pense passo a passo


Outro exemplo

Pergunta: Um diretor de cinema já dirigiu 16 filmes. Metade dos filmes que ele dirigiu são de ação e metade dos filmes de ação tem a participação do Nicolas Cage. Quanto filmes de ação com a participação do Nicolas Cage ele dirigiu?

Resposta: Vamos pensar passo a passo.

Se você não colocar vamos pensar passo a passo. Tem um grande probabilidade de dar errado pois ele vai embolar as informações.

Você pode fazer ele rever com mais cuidado

Prompt: Tem certeza? Reflita sobre a resposta.


https://platform.openai.com/docs/guides/gpt-best-practices

https://github.com/openai/openai-cookbook/blob/main/techniques_to_improve_reliability.md#maieutic-prompting

https://arxiv.org/abs/2201.11903

https://ai.googleblog.com/2022/05/language-models-perform-reasoning-via.html

https://arxiv.org/abs/2205.11916

https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/

CHAIN OF THOUGHT (CADEIA DE PENSAMENTO)

Utilize a lista de valores da planilha e o método Chain-of-Thought (Cadeia de raciocínio) no ChatGPT para obter o cálculo do valor do imposto a ser arrecadado. Considere que pessoas com rendimento de até R$20.000,00 pagam 10% de imposto, pessoas com rendimento entre R$20.000,00 e R$40.000,00 pagam 20% de imposto, e pessoas com rendimento acima de R$40.000,00 pagam 30% de imposto.



# AULA 04

Criar ferramentas usando API do gpt

Eightify - pega um vídeo transcreve o texto e resume usando chat GPT

Gamma.ap cria slides

JASPER - ai para criar propagandas


Você pode pedir para o GPT construir formulas para google sheets
Tenho uma planilha no Google sheets com notas de alunos. Na coluna A está o nome do aluno e na coluna B a nota. Crie uma fórmula para filtrar os alunos com notas acima de 7.

você pode pedir para que ele crie actions script para o google sheets:
Tenho uma planilha do Google sheets com uma lista de alunos e as notas de cada aluno em 4 diferentes provas. Quero uma função em APP Script para calcular a nota final do aluno. Ele recebe as 4 notas das provas e devolve uma nota com o seguinte critério: - Se o aluno tirou algum zero a nota final é 0.0 - se não a nota final é a média das 3 maiores notas.

OBS: No chatgpt o Enter funciona melhor que um ponto ou uma vírgula

```
function calcularNotaFinal(notal1, notal2, nota3, nota4){
    var notas = [nota1, nota2, nota3, nota4];
    notas.sort(function(a,b){return b - a;}) // ordena as notas em ordem decrescente

    if (notas[3] === 0){
        return 0.0;
    }else{
        var media = (notas[0] + notas[1] + notas[2])/3;
        return media.toFided(2); //retorna a média com duas casa decimais
    }
}
```
ele também te dar a forma de como usar

=calcularNotaFinal(B2, C2, D2, E2)

### Usar a API do GPT

Playground - você pode fazer testes

Maximum length - o número máximo de tokens que você quer (quanto mais mais caro)

Temperatura - Mede o grau de aleatoriedade da escolha do token. Se o valor for muito alto ele passa a criar fazes que não fazem sentido. Se a temperatura for zero ele tem uma grande chance de entregar a mesma resposta ou respostas levementes diferentes (por que o sevidor tem computadores paralelos rodando o algoritmo do GPT). Se você quer palavras inesperadas você almenta a temperatura.

System - Você cria regras para determinar como o assitente deve se comportar
Ex: você é um professo de física que escreve empaticamente com uso de gírias.
OBS: Nessa parte você deve retirar os vieses. No geral é mais puxado para homens brancos...


Ferramenta GPT TOKENIZER (site) - permite você visualizar quais são o tokens

(os tokens que você será cobrado são os tokens da pergunta e da resposta). Por isso você deve ser o mais certeiro possível na primeira mensagem.

```
const SECRET_KEY = "YOUR API KEY";
const MAX_TOKENS = 3000;
const TEMPERATURE = 0.9;

function EMAILALUNO(aluno, nota) {
  const url = "https://api.openai.com/v1/chat/completions";
  const payload = {
    model: 'gpt-3.5-turbo',
    messages: [
      { role: "system", content: "Crie um parágrafo de incentivo para um aluno que recebeu uma nota na prova. Vou passar o nome do aluno e a nota." },
      { role: "user", content: "Aluno: " + aluno + '. Nota: ' + nota },
    ],
    temperature: TEMPERATURE,
    max_tokens: MAX_TOKENS,
  };
  const options = {
    contentType: "application/json",
    headers: { Authorization: "Bearer " + SECRET_KEY },
    payload: JSON.stringify(payload),
    timeoutInSeconds: 60
  };
  const res = JSON.parse(UrlFetchApp.fetch(url, options).getContentText());
  return res.choices[0].message.content.trim();
}
```

OBS: Você deve pegar a sua apikey na ferramenta do chatgpt
plataformOpenAI.com

## Ferramentas geradoras de voz

## AUla 5

Usar o zapier para criar automação de email (no code)

Você programa quando acontecer algo você faz uma ação

Fazer um sistema que responde um email automaticamente usando o ChatGPT

Gmail -> New Email -> Conecte o Email -> Inbox -> (action) ChatGPT -> Conversation -> Conecte ao ChatGPT (API KEY) -> body Plain -> Assistant instruction (colocar o prompt). -> Apertar no + -> Gmail -> reply to Email -> trigger inbox -> custom (id da thread) -> insert data (resposta do assistente) (depois publish)


Desafios:

1. Automação de categorização de tweets em uma planilha do Google Sheets

Neste desafio, você deve criar um sistema automatizado para categorizar tweets em uma planilha do Google Sheets. A ideia é analisar campanhas de marketing nas redes sociais, especificamente aqueles que utilizam uma hashtag específica.

Sempre que alguém postar um tweet com essa hashtag no Twitter, o sistema deve adicionar automaticamente o tweet a uma planilha do Google Sheets e categorizá-lo como "Positivo", "Negativo" ou "Neutro". Isso permitirá a análise da recepção da campanha e a possibilidade de aprimorar a estratégia de marketing.

Você irá criar uma planilha no Google Sheets similar a esta, com as colunas "Usuário", "Tweet" e "Categoria". Depois, irá criar um novo Zap no Zapier, usando o Twitter como trigger (gatilho), e escolhendo a opção de busca por termo, utilizando a hashtag específica da campanha, como por exemplo #7DaysOfCode ou #ImersaoIA.

Feito isso, você poderá adicionar mais uma ação, que será usar o ChatGPT para categorizar o tweet como "Positivo", "Negativo" ou "Neutro". Por fim, você terá outra ação, que será para adicionar as informações do tweet na planilha do Google Sheets que você já criou (pode escolher a opção de criar múltiplas linhas na planilha), e você irá mapear cada coluna para seu item correspondente, que virão ou do Twitter ou do ChatGPT.

2. Análise automática de currículos

Você possui uma pasta no Dropbox onde os candidatos enviam seus currículos em formato PDF. Seu desafio é criar um fluxo automatizado que extraia os dados relevantes desses currículos e faça uma análise para determinar o nível de experiência de cada candidato.

Para isso, primeiramente você irá criar uma conta gratuita no PDF.co para acessar os dados de um PDF e converter arquivos PDF em texto, e obterá sua API KEY.

Em seguida, crie uma planilha no Google Drive similar a esta, com as colunas: "Nome completo", "Email", "Telefone", "Nível" e "Análise".

Com isso pronto, você irá começar um novo Zap no Zapier, e o trigger será a adição de um arquivo PDF a uma pasta sua no Dropbox. No app da PDF.co, configure o evento "PDF to Anything Converter" e insira sua API KEY. Defina o formato de saída como "Plain text without layout...". Preencha o campo "Source PDF URL" com o "1. Share link" do arquivo PDF no Dropbox. Selecione o idioma como "Portuguese".

Agora sim, você vai brincar com o ChatGPT. Você pode adicionar várias ações dele uma depois da outra. Cada ação irá extrair dados diferentes do texto do currículo:

Na primeira ação, extraia apenas o nome completo do candidato.
Na segunda ação, extraia apenas o email do candidato.
Na terceira ação, extraia apenas o telefone do candidato.
Na quarta ação, faça a análise do currículo. Avalie anos de experiência, projetos relevantes e tecnologias com as quais o candidato trabalhou. Classifique o nível do candidato como Júnior, Pleno ou Sênior.
Na quinta e última ação, analise a resposta anterior do ChatGPT e responda com uma palavra se o candidato é Júnior, Pleno ou Sênior.
Por fim, insira os dados extraídos na planilha criada usando uma ação do Google Sheets no Zapier (pode escolher a opção de criar múltiplas linhas na planilha).
