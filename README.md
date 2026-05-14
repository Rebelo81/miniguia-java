☕ Miniguia Java - NotebookLM
🎯 Contexto e Objetivos
Este repositório consolida meu projeto de estudo focado nos Fundamentos e Programação Orientada a Objetos (POO) em Java. A linguagem Java foi escolhida por sua forte presença no mercado, robustez para aplicações de médio e grande porte e seu consolidado ecossistema de bibliotecas
.
Objetivos de Estudo:
Compreender a arquitetura base da linguagem (JVM, JRE e JDK) e sua portabilidade (WORA)
.
Dominar a sintaxe básica, controle de fluxo e manipulação de tipos de dados
.
Aprofundar e aplicar os pilares da Programação Orientada a Objetos: Abstração, Encapsulamento, Herança e Polimorfismo
.
Utilizar IA (NotebookLM) para acelerar a curadoria, a síntese e a revisão dos conceitos técnicos.

--------------------------------------------------------------------------------
📚 Curadoria de Fontes
Para a construção desta base de conhecimento, o NotebookLM foi alimentado com 9 fontes variadas (entre vídeos, artigos e materiais universitários). Destaco as 5 principais utilizadas na construção deste guia:
Artigo DIO: Orientação a Objetos em Java: Conceitos Fundamentais - Cobertura direta dos pilares de POO
.
Apostila Caelum/ISPSN: Java e Orientação a Objetos - Exploração detalhada da máquina virtual, sintaxe, interfaces e bibliotecas (java.lang, java.io)
.
Artigo Dicas de Programação: Qual a diferença entre JDK, JRE e JVM - Esclarecimento didático da arquitetura de compilação e execução
.
Vídeo Fernanda Kipper: Curso de PROGRAMAÇÃO JAVA para INICIANTES - Guia prático de instalação, sintaxe e transição para POO
.
Apostila IME-USP: Introdução à Ciência da Computação com Java e Orientação a Objetos - Focada no histórico, laços de repetição, matrizes e boas práticas de código
.

--------------------------------------------------------------------------------
🛠️ Engenharia de Prompts e "Cicatrizes"
Documentação das iterações com a IA para extrair e refinar os resumos (Troubleshooting):
Tentativa 1 (Ampla): "Explique como o Java funciona e o que é POO."
Resultado/Cicatriz: A IA gerou um texto longo e misturado, sem separar claramente o papel do compilador e os conceitos de classes, perdendo a objetividade técnica.
Tentativa 2 (Estruturada): "Divida a explicação em dois tópicos: 1. A diferença exata entre JDK, JRE e JVM. 2. Defina os 4 pilares da POO (Encapsulamento, Herança, Polimorfismo e Abstração) em Java com base nas fontes."
Resultado: Resposta muito melhor. O modelo conseguiu isolar o funcionamento da Java Virtual Machine e listar os pilares da POO citando as fontes corretamente.
Tentativa 3 (Refinamento Prático): "Liste exemplos de como as fontes lidam com tratamento de erros (exceptions) e a diferença entre Vetores (Arrays) e Coleções (Lists, Sets)."
Resultado: Consegui extrair de forma clara as limitações de vetores tradicionais em comparação ao poderoso Java Collections Framework abordado pelas fontes da Caelum e UFMG.

--------------------------------------------------------------------------------
📖 Miniguia de Estudo (Entrega Final)
1. Resumos Estruturados do Assunto
A Arquitetura Java: WORA, JDK, JRE e JVM O sucesso do Java vem da sua capacidade de ser multiplataforma, baseada no conceito WORA (Write once, run anywhere - Escreva uma vez, execute em qualquer lugar)
. Para que isso funcione, a linguagem depende de três componentes centrais:
JDK (Java Development Kit): É o kit do desenvolvedor. Ele provê as ferramentas para programar, como o compilador javac, que transforma o arquivo de texto .java em um código intermediário chamado bytecode (.class)
.
JRE (Java Runtime Environment): É o ambiente de execução. Ele contém as bibliotecas padrão do Java (API core) necessárias para rodar um programa
.
JVM (Java Virtual Machine): É o coração da plataforma. Ela atua como um interpretador dinâmico que lê o bytecode e o traduz para instruções nativas do sistema operacional local (Windows, Linux, Mac), gerenciando também o isolamento de memória e coleta de lixo (Garbage Collector)
.
Sintaxe e Estruturas Fundamentais O Java é uma linguagem fortemente tipada, o que significa que o tipo de uma variável deve ser declarado explicitamente e não pode ser alterado durante a execução
.
Tipos Primitivos vs. Referência: Tipos primitivos (como int, double, boolean) guardam o valor diretamente na memória. Já os tipos de referência apontam para objetos (instâncias de classes) armazenados no heap
.
Estruturas de Controle: O fluxo do programa é ditado por condicionais como if/else e switch, e por laços de iteração (while, for) para evitar a repetição manual de código
.
Estruturas de Dados: Vai desde Arrays simples, que possuem tamanho fixo, até o uso avançado do Collections Framework, que disponibiliza implementações flexíveis como List (permite duplicados e mantém ordem), Set (não permite duplicados) e Map (associações chave-valor)
.
Programação Orientada a Objetos (POO) O Java força o programador a organizar o código em volta de Classes (moldes de atributos e comportamentos) e Objetos (entidades vivas geradas a partir das classes)
.
Encapsulamento: Oculta detalhes internos do objeto, protegendo modificações diretas através do uso de modificadores de acesso (private, public, protected) e liberando acesso via métodos getters e setters
.
Herança: Permite que uma classe filha herde atributos e métodos de uma superclasse usando a palavra-chave extends, promovendo grande reutilização de código
.
Polimorfismo: Capacidade de tratar objetos de diferentes classes de uma mesma forma (como por meio de uma Interface em comum), ou alterar o comportamento de um método nas subclasses usando @Override
.
Abstração: Foco apenas nas informações essenciais. Utiliza classes abstract (que não podem ser instanciadas) e interfaces (contratos que obrigam as classes a implementar determinados métodos)
.
2. Glossário
Bytecode: Código intermediário gerado pelo compilador Java (javac). Possui extensão .class e é lido pela Máquina Virtual Java em vez de ser lido diretamente pelo processador
.
Casting: Recurso utilizado para fazer a conversão explícita de um tipo de dado para outro no Java
.
Construtor: Um método especial invocado através do operador new no momento da criação de um objeto, utilizado para inicializar os atributos iniciais da instância
.
Exceptions (Exceções): Representadas por objetos da árvore Throwable, são mecanismos para tratamento de erros em tempo de execução, controlados por blocos try, catch e finally
.
Interface: Um "contrato" em Java que expõe o que um objeto deve fazer (assinaturas de métodos), sem especificar como ele deve fazer (implementação)
.
Javadoc: Ferramenta que gera documentação automática em formato HTML a partir de comentários estruturados no código fonte (iniciados com /**)
.
This: Palavra-chave que atua como uma referência ao próprio objeto durante a execução de seus métodos, ou chama a própria função construtora
.
Wrapper Classes: Classes no pacote java.lang (como Integer, Double, Boolean) que "empacotam" os tipos primitivos, permitindo que eles sejam tratados como objetos na memória
.
3. Prompts Reutilizáveis (Para Revisão)
Abaixo estão prompts formatados para você copiar e colar no NotebookLM ou qualquer outra IA, visando fazer testes ativos sobre seus conhecimentos:
Revisão de Arquitetura: "Crie um exercício de múltipla escolha com 5 perguntas sobre a diferença técnica entre JVM, JDK e JRE, e forneça o gabarito comentado ao final."
Revisão Prática de POO: "Gere um pequeno cenário do mundo real (como um sistema de biblioteca ou banco) e peça para eu identificar onde eu deveria usar Herança (extends) e onde eu deveria usar Interfaces (implements). Não me dê a resposta imediatamente, espere eu tentar resolver primeiro."
Explicador Analógico: "Explique o conceito de [INSERIR CONCEITO, ex: Polimorfismo] no Java usando uma analogia com situações do dia a dia, e em seguida mostre um pequeno trecho de código exemplificando a analogia."
Troubleshooting Simulado: "Me mostre um código em Java que tenta modificar uma variável 'private' sem usar um setter, ou que tente instanciar uma classe 'abstract'. Peça para eu encontrar o erro de compilação e sugerir a correção."
# miniguia-java
