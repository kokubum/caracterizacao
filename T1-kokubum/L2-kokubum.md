## Erick Silva Kokubum - T1-L1

# Caracterização da Linguagem Clojure

- Linguagem de Programação: <Clojure>

  - [Apresentação e histórico](#apresenta--o-e-hist-rico)
  - [Características da Linguagem](#caracter-sticas-da-linguagem)
  - [Capacidades da Linguagem](#capacidades-da-linguagem)
  - [Produtividade do Desenvolvedor](#produtividade-do-desenvolvedor)
  - [Ecossistema](#ecossistema)
  - [Informações Adicionais](#informa--es-adicionais)
  - [Referências](#refer-ncias)

## Apresentação e histórico

O Clojure é um dialeto da linguagem de programação Lisp, o criador do Clojure foi Rich Hickey, antes de desenvolver a linguagem ele trabalhou na dotLisp, em um projeto parecido com base na plataforma .NET, e também desenvolveu a interface jfli que é uma espécie de ponte para usar recursos do Java para Lisp Comum, o FOIL que é uma interface de objetos externos para Lisp e Lisplets que também é uma interface amigável do Lisp para o Java Servlets.

Todos esses projetos eram tentativas parar criar algum tipo de interoperabilidade entre Lisp e Java, mas Hickey gastou cerca de 2 anos e meio trabalhando na linguagem Clojure antes de lançá-la publicamente. Clojure é uma linguagem de programação de propósito geral com ênfase em programação funcional, ela é executa na (JVM) Máquina Virtual Java por padrão, mas também existem outras versões alternativas para outros ambientes de execução, como Clojure CLR, que compila o código para plataforma .NET e ClojureScript, que compila o código Clojure para o JavaScript, assim, como outros Lips, o Clojure trata o código como dados e tem um sistema de macros interligado.

Hickey gastou muito tempo trabalhando exclusivamente na linguagem e sem nenhum tipo de financiamento externo, no final desse período ele enviou um e-mail anunciando a linguagem para alguns amigos na comunidade Common Lisp, esse processo de desenvolvimento é voltado para a comunidade e o desenvolvimento é gerenciado no site da comunidade Clojure. O processo de desenvolvimento atual é conduzido pela comunidade e supervisionado por Rich Hickey como seu ditador benevolente perpétuo (BDFL em inglês).

## Características da Linguagem

- **Imutabilidade**

Não existe alteração de estado no paradigma funcional e no Clojure não poderia ser diferente. Temos no Clojure um conjunto de listas, vetores, sets e maps, todos imutáveis. Já que eles não conseguem adicionar ou remover nenhum valor dessas estruturas de dados, acabamos criando uma nova coleção com os valores antigos e o recente valor.

Outra vantagem da imutabilidade é a questão de testes. Contamos com um número bem menor de estados e transições para testar. Pela lógica, um sistema imutável é muito mais simples para testar totalmente.

Um dos problemas que o Java enfrenta, é quando um objeto é alterado, para tentar resolver isso temos sempre uma cópia da referência desse objeto. No Clojure já é bem diferente. Já que todos os estados são imutáveis, conseguimos compartilhar qualquer referência de objeto pois sabemos que não teremos problemas de alteração em nenhum objeto interno. O Clojure utiliza várias técnicas para salvar a memória, sendo uma das mais famosas a flyweight pattern.

- **High-Order function**

Uma High-Order function é uma função que ou aceita uma ou mais funções como argumento, ou retorna uma função como resultado. Esse é um dos conceitos fundamentais da programação funcional em qualquer linguagem.

Essas funções nos permitem criar outras funções, ou seja, conseguimos escrever pequenas funções que são combinadas para criar funções maiores. Seria como colocar um monte de pequenos blocos de LEGO juntos para a construção de uma casa.

- **First-Class functions**

Funções podem ser tratadas como valores na programação funcional. Dessa forma, conseguimos atribuir a valores que são passados para uma função, e que também são retornados por uma função.

As First-Class functions são essenciais para o estilo de programação funcional. Um exemplo disso é a função map, que espera receber no argumento uma função e uma lista, e retorna uma lista com o valores aplicados em cada membro da lista. Para que uma linguagem suporte o map, ela deve suportar a passagem de funções como argumento. Além disso, no Javascript também utilizamos a função map.

## Capacidades da Linguagem

Uma das vantagens de Clojure é ser uma linguagem mais objetiva. Enquanto em Java é preciso escrever muito código para dar uma instrução ao objeto, Clojure é mais conciso.

Outra vantagem está na hora de testar. Como programação funcional preza pelo princípio da imutabilidade, fica mais simples criar testes e garantir que elas funcionem conforme o esperado.

Além disso, por rodar em JVM, é possível utilizar todo o ecossistema criado para Java. Isso significa que, além de permitir o uso de bibliotecas de Java e facilitar a integração entre aplicações escritas nas duas linguagens, dá para aproveitar toda a base de código escrito em Java e integrá-la a uma aplicação escrita em Clojure.

## Produtividade do Desenvolvedor

O clojure possui como case de referência um dos maiores bancos digitais que é o Nubank, que ajuda cada vez mais nesse crescimento e evolução da própria linguagem na comunidade de desenvolvedores. Além disso, tal fator serve como uma influência incrivel no aumento e adesão a linguagem cada vez mais rápido.

## Ecossistema

Apesar de Clojure ser uma linguagem menos utilizada, sua comunidade é bem ativa – o que se traduz em maior e melhor suporte das pessoas e um ecossistema com ferramentas para automação de projetos, resolução de dependências, frameworks de propósitos gerais, entre outros.

## Informações Adicionais

---

## Referências

- [Clojure - Trybe](https://blog.betrybe.com/linguagem-de-programacao/clojure-tudo-sobre/)
- [Ninja do Linux - Clojure](http://ninjadolinux.com.br/clojure-introducao-a-linguagem/)
- [Codesh - Clojure](https://coodesh.com/blog/dicionario/o-que-e-clojure/)
