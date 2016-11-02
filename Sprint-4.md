# 1. Planejamento da Sprint
Não conseguimos entrar em contato com a Carla, por isso as estórias foram priorizadas pelo time na reunião de planejamento.

<b>
Em virtude do tempo de duração de sprint, definido em uma semana, estar se mostrando insuficiente à conclusão de User Stories devido à carga de trabalho demandada, a equipe definiu fazer uma subdivisão dos pontos definidos às User Stories em tarefas de forma a realizar o acompanhamento (Burndown, Velocity, EVM) mais granular, preciso e com menos dependências, sem comprometer a produtividade da equipe já habituada à agilidade semanal de produção.
</b>

## 1.1. Papéis

|Scrum Master|Product Owner|Development Team     |
|------------|-------------|---------------------|
|Lucas       | Jessica      |<ul><li>Allan</li><li>Elaine</li><li>Fabiola</li><li>Gustavo</li><li>Hugo</li><li>Luís</li><li>Pedro</li><li>Vitor</li>  |

## 1.2. Backlog

| US (User Story) | História | Pontuação |Nova Pontuação| Responsável |
|----------------------|----------|-----------|-----------|-----------|
|#7|Como um administrador, quero aprovar reservas de laboratórios solicitadas pelo corpo acadêmico para ter um maior controle sobre quem utiliza os laboratórios.|13|8|Pedro e Fabíola|
|#10|Como usuário, eu quero reservar um espaço a partir da tabela de ocupação para utilizar a sala.|---|8|Hugo e Luis|
|#11|Como administrador, eu quero designar um responsável pelas reservas que eu cadastrar para manter o controle da reserva.|---|13|Lucas e Vitor|

| TS (Technical Story) | História | Pontuação |Nova Pontuação| Responsável |
|----------------------|----------|-----------|-------------|--------------|
|#17 | Como desenvolvedor, eu quero fazer deploy para colocar o SAS em produção.|---| 2 | Gustavo|

###Débitos técnicos
| TS (Technical Story) | História | Pontuação |Nova Pontuação| Responsável |
|----------------------|----------|-----------|-------------|--------------|
| #10 | Como um desenvolvedor, eu quero realizar as validações necessárias da criação de reserva para garantir a consistência dos dados inseridos.|8|5|Elaine|
| #15 | Como um desenvolvedor, eu quero refatorar as views, para melhorar a qualidade do código. |13|---|Allan|
| #16 | Como desenvolvedor, eu quero refatorar a criação de reservas, para ficar mais intuitivo. |8|---|Gustavo|

As estórias técnicas TS#15 e TS#16 foram concluídas parcialmente, e como foi decidido anteriormente a equipe está acompanhando as tarefas, portanto seguem as tarefas que estão faltando dessas estórias para essa sprint.

#### Tarefa Pendente da História #15
| Tarefa | Pontuação | Responsável |
|--------|-----------|-------------|
| Diminuir complexidade da User View | 3 | Allan |

#### Tarefa Pendente da História #16
| Tarefa | Pontuação | Responsável |
|--------|-----------|-------------|
| Adaptar JavaScript| 4 | Gustavo |

## 1.3. Quadro de Conhecimentos
![Quadro de Conhecimentos](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/2_conhecimento.pn) 

## 1.4. Quadro de pareamento
![Quadro de Pareamento](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/2_pareamento.pn) 

## 1.5. Retrospectiva
|Pontos Positivos|
|----------------|


|Pontos Negativos |Causa| Melhoria|
|-----------------|-----|---------|

# 2. Resultados:

## 2.1. Burndown
![Burndown](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/2_burndown.pn)

## 2.2 Velocity
![Velocity](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/2_velocity.pn)

## 2.3 Agile EVM


## 2.4. Qualidade

### 2.4.1 Integração Contínua
![Coveralls](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/metrics/sprint2/travis.PN)

### 2.4.2 Cobertura de Testes
A cobertura de testes subiu de 68% na Sprint 1 para 82% na Sprint 2

![Coveralls](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/metrics/sprint2/coveralls.PN)

<hr>
<b>** Extrato Code Climate para Duplicação, Complexidade e PEP8 abaixo **</b>
![Coveralls](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/metrics/sprint2/code_climate.PN)

<b>** Identificação de Duplicação, Complexidade e PEP8 de acordo com as Issues**</b>
![Coveralls](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/metrics/sprint2/metrics.PN)

### 2.4.3 Duplicação de Código


### 2.4.4 Complexidade Ciclomática

### 2.4.5 Estilo: PEP8

### 2.4.6 Ações definidas para melhoria da qualidade