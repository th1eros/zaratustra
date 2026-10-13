# Zaratustra — The Art of Questioning

> **"Não confie cegamente no sistema. Compreenda-o."**

Um jogo filosófico e educacional sobre hacking, lógica, programação e segurança da informação, inspirado em *Assim Falou Zaratustra*, de Friedrich Nietzsche.

O objetivo não é derrotar inimigos, acumular poder ou completar batalhas. O objetivo é desenvolver uma mentalidade investigativa: aprender a questionar sistemas, compreender suas regras, formular hipóteses, testar possibilidades e construir conhecimento por meio da prática.

---

## 1. Visão geral

**Zaratustra** é um jogo de cartas investigativo, inicialmente executado no terminal, desenvolvido em C# com .NET 8 e organizado segundo o padrão arquitetural MVC (Model–View–Controller).

O projeto combina três pilares:

* **Filosofia:** questionamento, autossuperação, autonomia intelectual e criação de valores.
* **Hacking:** investigação de sistemas, análise de evidências, identificação de vulnerabilidades e compreensão de mecanismos computacionais.
* **Educação:** aprendizagem progressiva de C#, Linux, lógica, redes, programação e segurança da informação.

As cartas representam métodos de investigação e ferramentas intelectuais. Cada desafio funciona como um laboratório interativo, no qual o jogador precisa compreender um problema antes de propor uma solução.

O jogo deverá evoluir gradualmente de uma experiência textual para um ambiente com personagens, cenários e laboratórios mais complexos.

## 2. Premissa narrativa

O protagonista desperta em um sistema chamado **A Ordem**.

Nesse mundo, as regras estão estabelecidas, os processos são executados e as pessoas seguem instruções que raramente questionam. O sistema parece funcionar, mas ninguém consegue explicar completamente sua estrutura, suas contradições ou os motivos por trás de suas regras.

O protagonista recebe acesso a fragmentos desse mundo: registros, arquivos, documentos, mensagens de erro, políticas de acesso, terminais simulados e redes fictícias.

Cada fragmento contém informações necessárias para compreender o funcionamento de uma parte do sistema.

No início, o protagonista depende das pistas fornecidas. Com o avanço, aprende a distinguir fatos de suposições, reconhecer padrões, investigar inconsistências e desenvolver suas próprias hipóteses.

A jornada não consiste em destruir A Ordem, mas em compreendê-la.

O conflito central é intelectual: **o protagonista precisa decidir se continuará apenas seguindo instruções ou se desenvolverá a capacidade de compreender, questionar e transformar os sistemas dos quais participa.**

## 3. Fundamento filosófico

A principal inspiração filosófica é a obra *Assim Falou Zaratustra*, de Friedrich Nietzsche.

O jogo não pretende reproduzir literalmente o livro. Seus conceitos serão reinterpretados como elementos narrativos e pedagógicos.

### 3.1. A morte de Deus — a crise das certezas

No contexto do jogo, essa ideia representa o momento em que as explicações tradicionais deixam de ser suficientes.

O protagonista descobre que uma regra existir não significa que ela esteja correta, que um processo funcionar não significa que seja seguro e que uma autoridade declarar algo não substitui a verificação das evidências.

**Aplicação no jogo:** investigar regras, questionar premissas e verificar afirmações.

### 3.2. O além-do-homem — a superação das próprias limitações

O conceito de *Übermensch* inspira a evolução do protagonista para além da dependência de respostas prontas.

O progresso não será medido apenas pela quantidade de cartas obtidas, mas pela capacidade de resolver problemas novos com conhecimento adquirido anteriormente.

**Aplicação no jogo:** desafios progressivos, redução gradual das pistas e resolução independente de problemas.

### 3.3. As três metamorfoses

A transformação descrita por Nietzsche — camelo, leão e criança — servirá como estrutura para os estágios de aprendizagem.

**O Camelo — disciplina**

O jogador aprende os fundamentos, aceita desafios difíceis e desenvolve paciência para compreender os mecanismos básicos.

**O Leão — questionamento**

O jogador aprende a contestar premissas, identificar contradições e avaliar criticamente regras e sistemas.

**A Criança — criação**

O jogador combina conhecimentos, experimenta soluções e constrói novas ferramentas, métodos e interpretações.

Essas etapas representam uma adaptação pedagógica da obra, não uma classificação proposta por Nietzsche para hackers.

### 3.4. O eterno retorno — domínio real do conhecimento

A ideia do eterno retorno inspira a revisão e a reaplicação do conhecimento.

O jogador encontrará princípios já estudados em novos contextos. Um conceito compreendido superficialmente poderá exigir nova investigação quando aparecer em um cenário diferente.

**Aplicação no jogo:** revisão de conceitos, desafios recorrentes e testes de transferência de aprendizagem.

## 4. Princípios fundamentais do jogo

O projeto será orientado pelos seguintes princípios:

1. **Compreender antes de agir:** o jogador deve investigar o funcionamento de um sistema antes de propor alterações.
2. **Evidências antes de conclusões:** hipóteses precisam ser verificadas por observações e testes.
3. **Questionar sem abandonar o rigor:** desconfiar de uma afirmação não significa rejeitá-la automaticamente.
4. **Aprender por experimentação:** os conceitos serão ensinados por desafios práticos, não apenas por explicações.
5. **Autonomia intelectual:** o jogador deverá desenvolver a capacidade de resolver problemas sem depender continuamente de instruções.
6. **Responsabilidade técnica:** o conhecimento de segurança deve ser acompanhado pela compreensão de seus limites e consequências.
7. **Segurança por padrão:** os desafios serão executados em ambientes simulados ou laboratórios autorizados.

## 5. O sistema de cartas

As cartas são o principal mecanismo de interação durante a primeira versão do jogo.

Elas não representam ataques, armas ou habilidades de combate. Representam métodos de pensamento, técnicas de investigação e conhecimentos técnicos.

### 5.1. Categorias de cartas

| Categoria      | Função                          | Conhecimentos associados           |
| -------------- | ------------------------------- | ---------------------------------- |
| Observação     | Coletar e examinar informações  | Logs, evidências e observabilidade |
| Hipótese       | Formular explicações possíveis  | Lógica e método científico         |
| Privilégio     | Investigar permissões e acessos | Linux, autenticação e autorização  |
| Contradição    | Identificar inconsistências     | Depuração e análise de requisitos  |
| Análise        | Decompor sistemas em partes     | Algoritmos e arquitetura           |
| Experimentação | Testar hipóteses                | Testes, validação e depuração      |
| Abstração      | Identificar padrões gerais      | Programação e modelagem            |
| Criação        | Construir soluções próprias     | C#, automação e desenvolvimento    |

### 5.2. Exemplo de carta

**Carta: Observação**

* Categoria: Investigação
* Objetivo: coletar evidências antes de formular uma conclusão.
* Contexto: uma aplicação apresenta um erro inesperado.
* Ação: examinar as mensagens de erro e os registros disponíveis.
* Aprendizado: compreender a importância dos logs e da observabilidade.
* Critério de sucesso: identificar quais informações sustentam uma hipótese e quais ainda estão faltando.

As cartas poderão evoluir conforme o jogador demonstrar domínio dos conceitos relacionados.

## 6. Estrutura de um desafio

Cada laboratório seguirá um ciclo didático.

### Etapa 1 — Investigação

O jogador recebe um problema, um conjunto de evidências e informações incompletas.

### Etapa 2 — Formulação de hipóteses

O jogador utiliza cartas para selecionar possíveis explicações e definir quais informações precisa obter.

### Etapa 3 — Experimentação

O jogador executa ações simuladas, analisa dados, interpreta comandos ou escreve pequenos trechos de código.

### Etapa 4 — Verificação

O sistema compara o resultado com as condições esperadas e apresenta as evidências relevantes.

### Etapa 5 — Reflexão

O jogador recebe uma explicação da solução, compreende por que outras alternativas falharam e registra o conceito aprendido.

O sucesso dependerá da compreensão demonstrada, e não apenas da escolha correta de uma resposta.

## 7. Progressão educacional

A progressão será organizada para que o próprio desenvolvimento do jogo acompanhe a aprendizagem de programação e segurança.

| Fase               | Tema narrativo                           | Conteúdos técnicos                                      |
| ------------------ | ---------------------------------------- | ------------------------------------------------------- |
| 1. O Despertar     | Primeiro contato com A Ordem             | Terminal, entrada e saída em C#                         |
| 2. As Regras       | Compreender as decisões do sistema       | Variáveis, tipos, condicionais e lógica                 |
| 3. O Labirinto     | Investigar processos repetitivos         | Laços, métodos e algoritmos                             |
| 4. Os Arquivos     | Compreender informações persistentes     | Arquivos, diretórios e tratamento de erros              |
| 5. As Identidades  | Descobrir quem pode fazer o quê          | Usuários, grupos e permissões Linux                     |
| 6. A Rede          | Compreender a comunicação entre sistemas | IP, portas, DNS, TCP e HTTP                             |
| 7. As Contradições | Identificar falhas de implementação      | Depuração, validação e lógica de segurança              |
| 8. A Estrutura     | Compreender sistemas maiores             | POO, interfaces e arquitetura                           |
| 9. A Autonomia     | Resolver problemas desconhecidos         | Integração de conhecimentos e investigação independente |
| 10. A Criação      | Construir uma solução própria            | Desenvolvimento de ferramentas e projetos               |

A ordem poderá ser refinada conforme os desafios forem implementados. Cada fase deverá introduzir conceitos necessários para a seguinte.

## 8. Hacking como método de investigação

O jogo apresentará hacking como uma disciplina de compreensão e experimentação de sistemas.

O jogador deverá aprender a:

* Analisar o comportamento de programas.
* Formular hipóteses sobre falhas.
* Interpretar logs e mensagens de erro.
* Compreender permissões e controles de acesso.
* Identificar entradas inesperadas e condições de contorno.
* Investigar configurações incorretas.
* Entender protocolos e comunicação em redes.
* Reconhecer vulnerabilidades em aplicações de laboratório.
* Verificar se uma correção realmente resolve um problema.
* Documentar evidências, limitações e conclusões.

O foco será a aprendizagem técnica em ambientes controlados, com exercícios que ensinem tanto a identificação de problemas quanto sua prevenção e correção.

## 9. Arquitetura técnica

### Tecnologias iniciais

* **Linguagem:** C#
* **Plataforma:** .NET 8
* **Interface inicial:** terminal
* **Arquitetura:** MVC
* **Ambiente de desenvolvimento:** Visual Studio Code
* **Ambiente de execução planejado:** Linux

O projeto começará sem dependências externas desnecessárias. A prioridade é compreender a linguagem, a arquitetura e as regras do jogo antes de ampliar a infraestrutura.

### 9.1. Model

Responsável por representar os dados e o estado do jogo.

Exemplos:

* `Card`: define uma carta e suas propriedades.
* `Player`: representa o jogador e seu progresso.
* `Investigation`: representa uma investigação.
* `Evidence`: representa uma evidência coletada.
* `Hypothesis`: representa uma hipótese formulada.
* `Laboratory`: representa um desafio educacional.

### 9.2. View

Responsável por apresentar informações e receber a interação visual do jogador.

Exemplos:

* `GameView`: apresenta o estado geral do jogo.
* `CardView`: apresenta as cartas disponíveis.
* `InvestigationView`: exibe os documentos e as evidências.
* `LaboratoryView`: apresenta o desafio e seus resultados.

### 9.3. Controller

Responsável por coordenar as ações do jogador e o fluxo de interação.

Exemplos:

* `GameController`: coordena a execução do jogo.
* `InvestigationController`: coordena as investigações.
* `LaboratoryController`: coordena a execução dos desafios.

A lógica central deverá permanecer separada da apresentação, permitindo substituir o terminal por uma interface gráfica no futuro sem reescrever todas as regras.

**Observação arquitetural:** MVC organiza a interação e a apresentação, mas não substitui a separação das regras de domínio. Conforme o projeto crescer, a lógica dos laboratórios deverá permanecer independente da interface e dos controladores.

## 10. Evolução planejada

O desenvolvimento será incremental.

### Versão 0.1 — O Despertar

* Aplicação de console em C#.
* Menu inicial.
* Sistema básico de cartas.
* Primeiro laboratório investigativo.
* Registro do progresso durante a sessão.

### Versão 0.2 — Investigação

* Múltiplos laboratórios.
* Evidências e hipóteses.
* Feedback educacional.
* Desafios de lógica e depuração.

### Versão 0.3 — Conhecimento

* Progressão por competências.
* Cartas desbloqueáveis.
* Reaplicação de conceitos em novos contextos.
* Histórico de investigações.

### Versão 0.4 — O Sistema

* Laboratórios mais complexos.
* Simulação de arquivos, permissões e redes.
* Desafios de segurança defensiva.
* Maior integração entre programação e investigação.

### Versões futuras — O Mundo de Zaratustra

* Personagens com perspectivas filosóficas distintas.
* Cenários exploráveis.
* Narrativa ramificada.
* Interface gráfica.
* Laboratórios mais interativos.
* Possibilidade de integrar ferramentas técnicas em ambientes isolados e autorizados.

Essas etapas são uma visão inicial, não um compromisso de implementação de todos os recursos.

## 11. Segurança e limites operacionais

O objetivo educacional não exige colocar sistemas reais em risco.

Por isso, o projeto priorizará:

* Simulações locais e dados fictícios.
* Laboratórios isolados e autorizados.
* Ausência de ataques contra terceiros.
* Exercícios que ensinem identificação, validação e correção de vulnerabilidades.
* Separação entre os ambientes de simulação e os sistemas reais do usuário.

A segurança será um requisito de arquitetura, não um recurso adicionado posteriormente.

## 12. Objetivo final

Zaratustra pretende transformar o aprendizado de programação e segurança em uma jornada intelectual.

O jogador começa seguindo instruções. Depois, aprende a questionar. Finalmente, torna-se capaz de compreender sistemas, construir hipóteses, testar soluções e criar ferramentas próprias.

O projeto também servirá como ambiente de aprendizagem para seu desenvolvedor, que poderá estudar C#, .NET, arquitetura MVC, Linux, redes, lógica e segurança da informação enquanto implementa cada mecânica.

**O objetivo não é ensinar o jogador a decorar comandos. É ensiná-lo a compreender o que os comandos fazem, por que funcionam e em quais condições podem falhar.**

---

## Princípio fundador

> **O verdadeiro progresso não é obter mais ferramentas. É desenvolver a capacidade de compreender quando, por que e como utilizá-las.**

*Zaratustra — The Art of Questioning*
*Aprender. Investigar. Compreender. Criar.*