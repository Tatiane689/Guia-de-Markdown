# 2S - PTCC - Tatiane Carolina da Silva e Michael Santos Alves

# Guia de Markdown
Manual de referência do Markdown
---
Markdown é uma linguagem simples e leve para formatar texto, criada para ser fácil de escrever e ler, sem precisar de comandos complicados ou editores avançados.
Usar Markdown no GitHub facilita a formatação simples de texto, a criação de documentação clara, a visualização automática do conteúdo, a colaboração entre desenvolvedores e a criação de sites estáticos, tornando o gerenciamento de projetos mais eficiente.  
O Markdown é vantajoso para documentação e publicações porque é fácil de usar, permite criar textos bem organizados rapidamente, funciona bem em várias plataformas, e é simples de transformar em outros formatos, como HTML ou PDF. Também é fácil adicionar links, imagens e listas sem complicação.  
___

### Elementos Básicos do Markdown:
#### Cabeçalhos:

Em Markdown, os cabeçalhos são criados com o símbolo #. Quanto mais # você usar, menor será o nível do cabeçalho. Aqui estão os exemplos:

# Cabeçalho 1 (usando #)  
## Cabeçalho 2 (usando ##)  
### Cabeçalho 3 (usando ###)  
#### Cabeçalho 4 (usando ####)  
##### Cabeçalho 5 (usando #####)  
###### Cabeçalho 6 (usando ######)
---
#### Parágrafos:  
1.Para criar parágrafos, basta deixar uma linha em branco entre o texto. Por exemplo:

Este é o primeiro parágrafo.

Este é o segundo parágrafo.

2.Para uma quebra de linha (sem criar um novo parágrafo), você deve adicionar dois espaços no final da linha e pressionar "Enter". Exemplo:

Este é o primeiro parágrafo.  
Este é o mesmo parágrafo, mas com uma quebra de linha.
___
#### Linhas horizontais:  
Para criar uma linha horizontal (ou separador) em Markdown, basta usar três ou mais traços (-), asteriscos (*) ou underscores (_) em uma linha sozinha.  
Todos esses comandos criam uma linha horizontal que pode ser usada para separar seções no texto.
___
#### Comentários invísiveis:    
Tudo o que estiver dentro das tags <!-- e --> será ignorado pelo Markdown e não aparecerá na visualização.  
<!-- Este é um comentário invisível -->  
___
### Formatação de Texto:  
#### Ênfase (negrito, itálico, riscado):  
**Negrito**: Coloque o texto entre dois asteriscos (**).  
*Itálico:* Coloque o texto entre um asterisco (*).  
~~Riscado:~~ Coloque o texto entre dois tils (~~).  
Essas opções ajudam a destacar ou enfatizar partes do seu texto de forma simples.  
___  
#### Citações e blocos de citação:  
Para criar citações ou blocos de citação, você usa o sinal de > no início da linha. Isso cria um parágrafo destacado como uma citação.  
> Isso é uma citação.

Você pode adicionar múltiplas linhas para criar blocos de citação maiores:  
> Este é um bloco de citação.

> Ele pode ter várias linhas.

> E vai continuar como uma citação até o final.
___
#### Exibição de comandos no texto:  
Para exibir comandos dentro do texto em Markdown, você pode usar as seguintes sintaxes:  
Código em linha: Coloque o código entre crases simples (`).  
` comando `  
___
### Listas  
#### Listas ordenadas e não ordenadas:  
Para criar uma lista ordenada, você deve começar com um número seguido de um ponto (1., 2., etc.) e um espaço.  
Exemplo:  
1. Primeiro item
2. Segundo item
3. Terceiro item.

Para criar uma lista não ordenada, você pode usar três tipos de marcadores: um asterisco (*), um hífen (-), ou um sinal de adição (+), seguido de um espaço.  
Exemplo:  
* Item 1
* Item 2
* item 3

- Item 1
- Item 2
- Item 3

+ Item 1
+ Item 2
+ Item 3

#### Listas de Tarefas:  
Para criar uma lista de tarefas, você usa - [ ] para indicar uma tarefa não concluída e - [x] para indicar uma tarefa concluída.  
Exemplo:  
- [ ] Comprar açúcar  
- [x] Estudar Markdown  
- [ ] Ir ao mercado  

#### Listas com numeração não sequencial:  
Em Markdown, listas ordenadas normalmente seguem uma numeração sequencial, mas se você quiser criar uma lista com numeração não sequencial (ou seja, com números fora da ordem), o Markdown ainda renderiza a lista corretamente, ajustando os números automaticamente para refletir a ordem.  
Exemplo:  
1. Primeiro item
3. Terceiro item
2. Segundo item
5. Quinto item
4. Quarto item

O Markdown renderiza automaticamente a lista com a numeração sequencial correta.  
___
### Links e Referências:  
No Markdown, você pode facilmente adicionar links para sites externos ou criar referências para links internos ou externos, o que torna o conteúdo mais interativo.  
#### Links Simples:  
A sintaxe básica para criar um link no Markdown é: [Texto do link](URL)  
Exemplo:  
[Google](https://www.google.com) 

#### Links com referência:  
A ideia básica é definir o link em uma referência em algum lugar do documento e, depois, usar esse identificador para criar os links no texto.  
Exemplo:  
[Google][1]
[GitHub][2]

[1]: https://www.google.com
[2]: https://github.com  

___  
#### Criando âncoras para navegação no documento:  
No Markdown, você pode criar âncoras para navegação dentro do mesmo documento. Isso é útil para guiar o usuário para seções específicas, especialmente quando você tem um documento longo com várias seções. As âncoras funcionam basicamente como links internos que levam o usuário para uma parte do conteúdo.  
Para criar uma âncora, você utiliza um link de ancoragem que aponta para um título de seção do seu documento. O título da seção será automaticamente convertido para uma ID e, em seguida, você cria um link que aponta para essa ID.  

**Passos:**  
1. Defina um título de seção com # (para títulos de nível 1, 2, 3, etc.).
2. Crie um link para essa seção utilizando a ID do título (que é automaticamente gerada).

##### Sintaxe para Criar uma Âncora:  
- O Markdown automaticamente converte os títulos em IDs com base no texto do título, removendo espaços e convertendo as letras para minúsculas.
- As palavras do título são separadas por hífens.
Por exemplo, se você tiver um título como:
## Minha Seção Importante  
A ID gerada será minha-seção-importante.  
###### Criando a Navegação para a Âncora  
Você cria o link para essa seção usando a ID gerada, precedida por #:  
[Ir para Minha Seção Importante](#minha-seção-importante)  
Exemplo Completo:  
# Título Principal

Este é o início do documento.

## Seção 1
Conteúdo da Seção 1.

## Seção 2
Conteúdo da Seção 2.

[Ir para Seção 1](#seção-1)  
[Ir para Seção 2](#seção-2)  
#### Explicação:  
1. O título ## Seção 1 será automaticamente convertido para a ID seção-1.
2. O título ## Seção 2 será convertido para seção-2.
3. Os links [Ir para Seção 1](#seção-1) e [Ir para Seção 2](#seção-2) irão levar o usuário diretamente para essas seções dentro do documento.

___
### Imagens e Mídias:  
#### Imagens externas:  
No Markdown, você pode facilmente adicionar imagens e mídias (como vídeos e outros tipos de mídia) ao seu documento.  
A sintaxe básica para adicionar imagens no Markdown é:  
![Texto alternativo](URL da imagem)  
**Texto alternativo:** É um texto que será exibido caso a imagem não carregue. Além disso, é importante para a acessibilidade.  
**URL da imagem:** O caminho para a imagem, que pode ser um caminho local ou um link direto para uma imagem hospedada na web.  
Exemplo:  
![Logo do GitHub](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)  

#### Imagens locais:  
Imagens locais são aquelas que estão no mesmo diretório ou em um diretório relativo ao arquivo Markdown. A diferença é que, em vez de usar uma URL, você especifica o caminho do arquivo local.  
**Sintaxe:**  
![Texto alternativo](caminho/para/a/imagem.extensão)  
Exemplo de Imagem Local:  
Se a imagem estiver no mesmo diretório do arquivo Markdown:  
![Imagem Local](minha-imagem.jpg)  
Se a imagem estiver em um diretório específico, como imagens/:  
![Imagem Local](imagens/minha-imagem.jpg)  
**Resultado:** (Se a imagem minha-imagem.jpg estiver presente no diretório correto, ela será exibida).  

#### Criando imagens clicáveis (com links):  

Em Markdown, você pode criar imagens clicáveis, ou seja, imagens que funcionam como links. Para fazer isso, você combina a sintaxe de link com a sintaxe de imagem.  
**Sintaxe para Imagem Clicável:**  
A estrutura básica para criar uma imagem clicável é envolver a imagem dentro de um link. A sintaxe é a seguinte:  
[![Texto alternativo](URL da imagem)](URL do link)  
**Explicação:**  
1. [![Texto alternativo](URL da imagem)]: Este é o formato de uma imagem. A imagem é mostrada, e o texto alternativo será exibido caso a imagem não carregue.
2. (URL do link): O link para o qual a imagem será clicável.

**Exemplo de Imagem Clicável:**  

[![Logo do GitHub](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)](https://github.com)  
___
### Trabalhando com Código  
#### Código inline e em blocos:  
O **código inline** é usado quando você deseja incluir pequenos trechos de código ou comandos dentro de uma frase ou parágrafo, sem quebrar o fluxo do texto.  
**Sintaxe para Código Inline:**  
Para criar código inline, você usa backticks (crase) ` ao redor do código.  
Exemplo:  
O comando para listar arquivos no Linux é `ls`.  

O **bloco de código** é utilizado quando você precisa destacar grandes trechos de código ou** quando o código precisa ser exibido em múltiplas linhas. Em Markdown, você pode usar blocos de código de duas maneiras: com indentação ou com três backticks. 

**Bloco de Código com Três Backticks**  
A maneira mais comum e recomendada de criar blocos de código em Markdown é utilizando três backticks ``` antes e depois do código. Você também pode especificar a linguagem de programação após os três backticks para destacar a sintaxe.  
**Sintaxe para Bloco de Código:**  
```linguagem
Seu código aqui
```
Exemplo de bloco de código em Python:  
```markdown
```python
def saudacao():
    print("Olá, mundo!")
saudacao()
```
**Bloco de Código com Indentação**  
Uma alternativa (menos comum) para criar blocos de código é usar indentação de quatro espaços ou um tab no início de cada linha de código.  
**Sintaxe com Indentação:**  
 def saudacao():
        print("Olá, mundo!")
    saudacao()  
___
### Elementos Avançados  
#### Tabelas e alinhamentos:  
Em Markdown, você pode criar tabelas de forma simples, e também é possível controlar o alinhamento do conteúdo nas células. As tabelas são úteis para exibir dados de maneira organizada, como em listas, comparações, ou informações estruturadas.  

**Criando Tabelas**  
Uma tabela no Markdown é criada usando pipe (|) para separar as colunas e hífen (-) para criar a linha de cabeçalho.
**Sintaxe Básica de Tabelas:**  
| Cabeçalho 1 | Cabeçalho 2 | Cabeçalho 3 |
|-------------|-------------|-------------|
| Dado 1      | Dado 2      | Dado 3      |
| Dado 4      | Dado 5      | Dado 6      |  

**Exemplo de Tabela Simples:**  
| Nome       | Idade | Cidade      |
|------------|-------|-------------|
| João       | 25    | São Paulo   |
| Maria      | 30    | Rio de Janeiro |
| Pedro      | 28    | Belo Horizonte |

**Alinhamento das Colunas**  
Você pode controlar o alinhamento do conteúdo de cada coluna usando dois pontos (:) ao lado dos hífens na linha de cabeçalho.
**Alinhamento à Esquerda:**  
Para alinhar o conteúdo à esquerda, coloque os dois pontos à esquerda do hífen:  
| Alinhamento Esquerda |
|:---------------------|
| Texto 1              |
| Texto 2              |  

**Alinhamento ao Centro:**  
Para alinhar o conteúdo ao centro, coloque os dois pontos de ambos os lados do hífen:  
| Alinhamento Centro |
|:------------------:|
| Texto 1            |
| Texto 2            |  

**Alinhamento à Direita:**  
Para alinhar o conteúdo à direita, coloque os dois pontos à direita do hífen:  
| Alinhamento Direita |
|---------------------:|
| Texto 1             |
| Texto 2             |  

**Exemplo Completo de Tabela com Alinhamento:**  
Você pode combinar todos os tipos de alinhamento na mesma tabela.  
| Nome      | Idade | Cidade          |
|:----------|------:|:---------------:|
| João      |    25 | São Paulo       |
| Maria     |    30 | Rio de Janeiro  |
| Pedro     |    28 | Belo Horizonte  |  

___

### Notas de rodapé:  
Em Markdown, o suporte para notas de rodapé não é uma parte do padrão oficial, mas muitas implementações de Markdown (como no GitHub ou Pandoc) permitem adicionar notas de rodapé de forma simples e eficaz. O objetivo das notas de rodapé é fornecer informações adicionais sem sobrecarregar o conteúdo principal do texto.  
A sintaxe de notas de rodapé no Markdown segue o padrão abaixo:  
Você usa colchetes duplos [^1] para criar um marcador de nota de rodapé.  
A nota de rodapé em si é criada no final do documento, usando a mesma chave, mas com o conteúdo explicativo após o :.  
**Exemplo:**  
Aqui está um exemplo de uma afirmação que precisa de uma explicação[^1].

[^1]: Esta é a explicação ou a fonte que será exibida como uma nota de rodapé.  

___

### Emojis e badges  

Emojis podem ser usados diretamente no texto usando seu código de Unicode ou os códigos curtos de emojis suportados por muitas plataformas de Markdown.  
Em plataformas como GitHub, você pode usar os códigos curtos para emojis, que são rodeados por dois pontos (:). Por exemplo, o código para o emoji de coração é :heart:.  
**Exemplo:**  
Eu adoro Markdown! :heart:  

Badges são pequenos ícones que geralmente exibem o status de algum atributo de um projeto, como build, cobertura de código, versão ou licença. Normalmente, você verá badges em repositórios de código, como no GitHub, onde essas imagens ajudam a fornecer informações úteis sobre o status do projeto.  
**Badges de Serviços Externos**  
Vários serviços oferecem badges prontos para usar, como Travis CI, CircleCI, Coveralls, e Shields.io. Esses badges podem ser facilmente inseridos em seu documento Markdown.  
A sintaxe básica para adicionar um badge de imagem em Markdown é:  
![Texto Alternativo](URL-da-imagem)  

**Exemplo de Badge de Build (Travis CI)**  
Por exemplo, se você quiser adicionar um badge de status de build do Travis CI, você pode usar o seguinte código:  
![Build Status](https://travis-ci.org/usuário/projeto.svg?branch=main)  

**Exemplo de Badge com Shields.io**  
O Shields.io oferece uma maneira fácil de gerar badges personalizados para status de projetos, versões, downloads, entre outros.  
![Version](https://img.shields.io/badge/version-v1.0.0-brightgreen)  

**Badges de Licença**  
Aqui está um exemplo de um badge de licença, que indica sob qual licença o projeto está sendo distribuído:  
![License](https://img.shields.io/badge/license-MIT-blue)  

___  

### Integração com HTML para personalização  
Você pode adicionar elementos HTML diretamente dentro de um arquivo Markdown para personalizar a formatação.  
**Exemplo:** Usando <div> e <span>  
Este é um exemplo de texto normal.

<div style="color: red; font-weight: bold;">
    Este texto está em vermelho e negrito.
</div>

<span style="font-size: 20px; color: green;">Texto em verde e tamanho maior</span>  

**Inserindo Imagens com HTML**  
Embora o Markdown tenha uma sintaxe para imagens, você pode usar HTML para personalizar as imagens de forma mais detalhada, como adicionar largura, altura, bordas e margens.  
**Exemplo:** Imagem com HTML  
<img src="https://example.com/imagem.jpg" alt="Exemplo" width="300" height="200" style="border-radius: 10px;">  

___  
### Publicação no GitHub  

**Criando um Novo Repositório**  
1. Faça login na sua conta GitHub.
2. Na página inicial, clique no ícone de + no canto superior direito e selecione New repository
3. Preencha as informações do seu repositório:
- Repository name (Nome do repositório): Escolha um nome único para o seu repositório.
- Description (Descrição): Opcional, uma breve descrição sobre o que o repositório vai conter.
- Public ou Private: Escolha se o repositório será público (qualquer pessoa pode ver) ou privado (somente você e convidados podem acessar).
- Initialize this repository with a README: Se você marcar essa opção, o GitHub criará automaticamente um arquivo README.md no repositório.
- Add .gitignore: Se você deseja adicionar um arquivo .gitignore que exclui arquivos desnecessários do repositório, pode escolher um template baseado na linguagem ou ferramenta que você está usando.
- Choose a license: Se você deseja adicionar uma licença ao seu repositório, pode escolher uma licença aqui (como MIT, GPL, etc.).
4. Clique em Create repository para finalizar.


**Enviando o arquivo Markdown**

Para enviar um arquivo Markdown para um repositório no GitHub, você pode seguir os passos abaixo. Isso envolve adicionar ou criar o arquivo Markdown no seu repositório local e, em seguida, enviá-lo para o GitHub.  

1. Crie o arquivo Markdown e salve com a extensão .md.
2. Coloque o arquivo dentro do diretório do seu repositório local.
3. Adicione o arquivo ao Git com git add.
4. Comite as alterações com git commit.
5. Envie para o GitHub usando git push.

**Visualizando o documento diretamente no GitHub**  

uando você envia um arquivo Markdown (.md) para um repositório no GitHub, ele é automaticamente renderizado na plataforma. Isso significa que, ao acessar o arquivo no repositório, você verá o conteúdo formatado, com títulos, listas, links, imagens e código exibidos de forma organizada e legível.  

**Passos:**  
1. Envie o arquivo Markdown para o seu repositório no GitHub.
2. Acesse o repositório e clique no arquivo Markdown.
3. O GitHub renderiza automaticamente o arquivo, mostrando-o de forma formatada.








