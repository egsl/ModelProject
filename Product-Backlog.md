## 1. Introdução
O presente documento apresenta todas as histórias técnicas e de usuário a serem realizadas durante a _Release 2_ do projeto SAS (Sistema de Alocação de Salas). Tais histórias foram pontuadas de acordo com seu nível de complexidade, resultando em um total planejado de **155 pontos**.

## 2. Histórias de usuário

|Issue|US (User Story) | História | Pontuação |
|-----|----------------|----------|-----------|
|[#17](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/17) | #1 | Como um administrador, quero consultar os dados de todos os usuários cadastrados no sistema. | 13 | 
|[#18](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/18)  | #2 | Como um administrador, quero consultar todas reservas já efetuadas visualizando todos dados. | 8 |
|[#20](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/20) | #3 | Como um usuário, quero excluir as reservas feitas por mim. | 5 | 
|[#21](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/21) | #4 | Como administrador, quero excluir qualquer reserva efetuada. | 8 |
|[#22](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/22) | #5 | Como um usuário, quero consultar a disponibilidade e as reservas já realizadas em determinado espaço. | 20 |
| [#23](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/23) | #6 | Como um administrador, quero gerenciar administradores do sistema de modo que consiga tornar um usuário do corpo acadêmico em administrador. | 13 |
|[#24](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/24)  | #7 | Como um administrador, quero aprovar reservas de laboratórios solicitadas pelo corpo acadêmico. | 13 |
|[#25](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/25) | #8 | Como um visitante, quero consultar as perguntas frequentes do sistema. | 3 |
|[#26](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/26) | #9 | Como um administrador, quero visualizar relatórios de reserva de modo que possa identificar os espaços mais utilizados em determinados períodos. | 20 |

## 3. Histórias técnicas (teste e refatoração)

|Issue|TS (Techinical Story) | História | Pontuação |
|-----|----------------|----------|-----------|
|[#3](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/3)  | #1 | Como um desenvolvedor, eu quero criar um app de usuário para melhorar a gerência dos usuários. | 3  |
|[#4](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/4)  | #2 | Como um desenvolvedor, eu quero realizar as validações necessárias do cadastro de usuário para garantir a consistência dos dados inseridos. | 5  |
|[#5](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/5) | #3 | Como um desenvolvedor, eu quero testar o cadastro de usuário para garantir a funcionalidade do método.| 3 |
|[#6](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/6) | #4 | Como um desenvolvedor, eu quero realizar as validações necessárias da alteração de usuário para garantir a consistência dos dados inseridos. | 3 |
|[#7](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/7) | #5 | Como um desenvolvedor, eu quero testar a alteração de usuário para garantir a funcionalidade do método. | 3 |
|[#8](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/8) | #6 | Como um desenvolvedor, eu quero testar a exclusão de usuário para garantir a funcionalidade do método. | 2 |
|[#9](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/9) | #7 | Como um desenvolvedor, eu quero testar a consulta de usuário para garantir a funcionalidade do método. | 2 |
|[#10](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/10) | #8 | Como um desenvolvedor, eu quero realizar as validações necessárias do login de usuário para garantir a consistência dos dados inseridos. | 2 |
|[#11](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/11) | #9 | Como um desenvolvedor, eu quero testar o login e logout de usuário para garantir a funcionalidade do método. | 3 |
|[#12](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/12) | #10 | Como um desenvolvedor, eu quero realizar as validações necessárias da criação de reserva para garantir a consistência dos dados inseridos. | 8 |
|[#13](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/13) | #11 | Como um desenvolvedor, eu quero testar a criação de reserva para garantir a funcionalidade do método. | 5 | 
|[#14](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/14) | #12 | Como um desenvolvedor, eu quero refatorar o cadastro de criação de reserva para consertar os bugs conhecidos. | 8 |
|[#16](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/issues/16) | #13 | Como um desenvolvedor, eu quero testar a consulta de reserva para garantir a funcionalidade do método. | 5 |