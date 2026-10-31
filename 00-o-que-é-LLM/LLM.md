# O que é um modelo de linguagem ou LLM?

# Introdução

Hoje vamos entender como um LLM recebe um pedido, gera uma resposta e qual é seu papel em um agente de IA.

---

## O que é?

**LLM** é a sigla de **Large Language Model** (modelo de Linguagem de grande porte). É um modelo treinado para processar sequências de tokens e gerar respostas conforme a mensagem recebida.

Muitos LLMs são **modelos fundacionais** (foundation models), treinados com grandes volumes de dados para realizar ou serem adaptados a diferentes tarefas. Também existem modelos fundacionais que trabalham com imagens, áudio e outros tipos de dados, são modelos multimodais.

---

## O treinamento de um modelo

É o processo em que ele aprende padrões a partir de dados. Durante esse processo, são ajustados seus **parâmetros**, que são valores numéricos internos que influenciam como o modelo processa informações e gera respostas. Esse treinamento pode envolver diferentes etapas e métodos: Pré-treinamento, ajuste fino, treinamento por preferências ou reforço.

> Nem todos os modelos utilizam as mesmas etapas ou métodos. Por exemplos, modelos criados para gerar código podem ser treinados com todos os repositórios públicos do github e todas as perguntas e respostas do stack overflow.

Ao receber um prompt, o LLM utiliza os padrões aprendidos e o contexto fornecido para gerar textos, códigos ou formatos estruturados.

---

## O que pode fazer sozinho?

Com base no contexto recebido (prompt do usuário) e nos padrões aprendidos no treinamento, um LLM pode:

- Responder a perguntas com base no contexto e no que aprendeu no treinamento.
- Explicar conceitos e reformular textos.
- Resumir, traduzir e classificar textos.
- Criar rascunhos, exemplos e ideias.
- Gerar código ou dados estruturados conforme as instruções.
- Analisar informações apresentadas e sugerir possíveis soluções.

## O que não pode fazer sozinho?

- Pesquisar na internet.
- Editar um arquivo.
- Responder com dados atualizados após seu treinamento.
- Manter histórico de uma conversa.

---

## Como funciona?

**Passo 1:**

O usuário escreve uma mensagem e envia ao modelo:

```plaintext
Me explique em uma frase o que é uma LLM
```

**Passo 2:**

O modelo divide a mensagem em vários tokens:

> **Tokens:** são unidades usadas pelo modelo para processar texto; uma palavra pode ser dividida em vários tokens. Cada modelo tem suas regras de divisão e quebra de token.

Exemplo:

![imagem mostrando um site que exibe uma mensagem de um usuario e como o modelo quebra em tokens](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/6v9ibqwwi9hz94iymrwk.png)

[Link para a ferramenta](https://tokenvisualizer.netlify.app/)

**Passo 3:**

O modelo usa os parâmetros de treinamento para de forma matemática determinar quais tokens ele pode devolver para gerar uma resposta satisfatória.

![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/1u8gcl1qhq2gnt2beouh.png)

**Passo 4:**

O modelo devolve a resposta para o usuário em linguagem natural:

```plaintext
Uma LLM é um modelo de inteligência artificial que processa e gera textos.
```

---

## Qual a diferença entre um LLM e um agente de IA?

Um **LLM** recebe um contexto e produz uma saída. Já um **agente de IA** combina esse modelo com um fluxo de trabalho que pode usar ferramentas da aplicação para realizar uma ou mais tarefas em uma ou mais etapas, inclusive salvando o contexto da conversa.

![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/lf1onn2pkp5uannxqbmk.png)

### Exemplos de LLM

- GPT-4 (OpenAI).
- Claude Sonnet 4.5 (Anthropic).
- Gemini 2.5 Pro (Google).

### Exemplos de agentes de IA

- Claude code (Anthropic).
- Codex (OpenAI).
- Copilot (Microsoft).


### Um exemplo prático

você pergunta:

```plaintext
Qual é a temperatura em São Paulo agora?
```
**Resposta com o modelo LLM**

O modelo pode gerar uma resposta com base no que aprendeu durante o treinamento, mas, sem acesso a dados atualizados, não consegue confirmar a temperatura atual.

**Resposta com o agente**

O agente identifica que precisa de informações atualizadas, faz consulta a uma ferramenta de previsão do tempo e retorna a temperatura informada naquele momento.

**A diferença:** o LLM gera respostas com base nos padrões aprendidos e no contexto recebido, enquanto o agente pode utilizar ferramentas para consultar informações externas e assim executar ações.

---

## Conclusão

Podemos comparar o **LLM a um cérebro**, que processa informações, interpreta e gera respostas a partir dos seus padrões matemáticos aprendidos. Dá mesma forma que um ser humano só consegue responder sobre assuntos que aprendeu durante a vida.

E quando um humano inventa algo que não sabe só para responder uma pergunta? Parabéns você entendeu o que é a alucinação da LLM.

Até o próximo artigo :)

## Referências

* Huyen, C. (2026). [Engenharia de IA: Construindo aplicações com modelos de fundação](https://novatec.com.br/livros/engenharia-de-ia/). Novatec Editora.
* Albada, M. (2026). [Construindo Aplicações com Agentes de IA](https://novatec.com.br/livros/construindo-aplicacoes-com-agentes-IA/). Novatec Editora.

## Publicações

* Link do artigo publicado [Dev.to ](https://dev.to/paula-figueiredo/ia-para-devs-02-o-que-e-um-modelo-de-linguagem-ou-llm-5677)
