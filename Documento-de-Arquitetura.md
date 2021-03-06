# Histórico de revisões deste documento

|Data|Versão|Descrição|Autor|
|----|------|---------|-------|
|26/08/2016 |1.0 | Introdução |Vítor |
|26/08/2016 |1.1 | Visão Geral da Visão Lógica |Fabíola |
|27/08/2016 |1.2 | Visão de Casos de Uso |Hugo |
|27/08/2016 |1.3 | Qualidade |Vítor |
|27/08/2016 |1.4 | Atualizando Visão de Casos de Uso |Hugo |
|28/08/2016 |1.5 | Atualizando Visão Lógica|Fabíola |
|30/08/2016 |1.6 | Representação Arquitetural |Lucas |
|30/08/2016 |1.6 | Atualizado Representação Arquitetural |Lucas |
|30/08/2016 |1.7 | Restrições e Metas Arquiteturais |Luis |
|30/08/2016 |1.7 | Inclusão das Prioridades de caso de uso |Fabíola e Lucas |
|31/08/2016 |1.8 | Inclusão do Diagrama de Classe |Luis |
|31/08/2016 |1.9 | Atualizando Visão de Casos de Uso |Hugo |
|31/08/2016 |2.0 | Visualização da Implantação |Hugo |
|01/09/2016|2.1 | Atualizando a Visão Lógica |Fabíola |
|01/09/2016|2.2 | Atualizando a Visão de Casos de Uso |Fabíola |
|02/09/2016|2.3 | Atualizando Restrições e Metas Arquiteturais |Luis |
|04/09/2016|2.4 | Remoção da Visualização da Implantação|Hugo |
|11/09/2016|2.5 | Atualizando Visão Geral e Inclusão da Visão em Camadas|Luis |
|11/11/2016|2.6 | Atualizando Diagrama de Pacotes|Fabíola |

#Índice


[1. Introdução](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/wiki/Documento-de-Arquitetura#1-introdu%C3%A7%C3%A3o)

[2. Representação Arquitetural](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/wiki/Documento-de-Arquitetura#2-representa%C3%A7%C3%A3o-arquitetural)

[3. Restrições e Metas Arquiteturais](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/wiki/Documento-de-Arquitetura#3-restri%C3%A7%C3%B5es-e-metas-arquiteturais)

[4. Visão de Casos de Uso](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/wiki/Documento-de-Arquitetura#4-vis%C3%A3o-de-casos-de-uso)

[5. Visão Lógica](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/wiki/Documento-de-Arquitetura#5-vis%C3%A3o-l%C3%B3gica)

[6. Visão da Implementação](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/wiki/Documento-de-Arquitetura#6-vis%C3%A3o-da-implementa%C3%A7%C3%A3o)

[7. Qualidade](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/wiki/Documento-de-Arquitetura#7-qualidade)
# 1. Introdução

Esta seção apresenta uma visão ampla deste Documento de Arquitetura, apontando sua finalidade e abrangência, bem como definições, acrônimos, abreviações utilizadas dentro do mesmo.

## 1.1. Objetivo

Este documento expõe a arquitetura do Sistema de Alocação de Salas (SAS) de maneira abrangente, pontuando aspectos deste segundo diferentes visões arquiteturais. Além disso, exprime-se decisões significativas adotadas segundo a arquitetura em relação ao sistema.

## 1.2. Escopo

O Documento de Arquitetura descreve o sistema, ajudando na compreensão de seu comportamento, sendo, assim, um meio de avaliar se a abordagem utilizada atende aos requisitos do cliente. Ele tem como base o Documento de Visão e afeta diretamente as ferramentas utilizadas e a implementação do sistema.

## 1.3. Definições, Acrônimos e Abreviações

* MVC: Model-View-Controller (Modelo-Visão-Controladora, em inglês) 
* MTV: Model-Template-View (Modelo-Template-Visão, em inglês)


# 2. Representação Arquitetural

A arquitetura utilizada será a arquitetura do Django que tem como padrão a MVC. A camada de modelo (Model) é responsável pelas classes de domínio, pela leitura e escrita de dados e pela comunicação com o banco de dados. A camada de visão (View) é responsável pela interface com o usuário, ou seja, é ela que faz a apresentação da aplicação. E a camada de controle (Controller) é responsável por trabalhar com as requisições e fazer o controle em si da aplicação.

![MVC ](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/MVC.png)

# 3. Restrições e Metas Arquiteturais

## Suportabilidade
* A principal plataforma para o uso do sistema será o Google Chrome. Assim, sistema deverá ser compatível com a versão 52 ou superior

## Usabilidade
* O sistema deve ser simples e intuitivo. Deve possibilitar que novos usuários aprendam a usá-lo sem necessitar de ajuda

## Ferramentas de Desenvolvimento
* A linguagem utilizada para o desenvolvimento do sistema será o Python (versão 3.4.3) e o framework Django (versão 1.10)

## Confiabilidade
* Para garantir a qualidade e que o sistema foi suficientemente testado, o sistema deve ter uma cobertura de testes, mínimo de 90%

# 4. Visão de Casos de Uso

## 4. 1.  **Atores**  

### 4. 1. 1. **Visitante**  
Este ator é um usuário do sistema que não realizou login ou não possui cadastro que pode consultar reservas e visualizar relatórios.  

### 4. 1. 2. **Administrador**  
Este ator administra as reservas de sala, o corpo acadêmico e administradores.   

### 4. 1. 3. **Corpo Acadêmico**  
Este ator realiza atividades (consultar, reservar, cancelar) relativas a reservas.
  
## 4. 2. **Diagrama de casos de uso**  
![Imagem - Diagrama de Casos de Uso](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/CasoUso.png)  

## 4.3. Prioridade dos casos de uso
Os casos de uso possuem três tipos de prioridades, são elas:

* Essenciais: São aqueles que são indispensáveis para o sistema. 
* Importantes: São recursos necessários para o cliente mas o sistema pode funcionar sem eles.
* Desejáveis: Sem estes recursos o sistema já atende as necessidades do cliente, podem ser adicionados posteriormente.

|Identificador|Caso de Uso|Prioridade|
|----|------|---------|
|UC01 |Manter usuário | Essencial |
|UC02 |Realizar login | Essencial |
|UC03 |Criar reserva |Essencial |
|UC04 |Consultar reserva |Essencial |
|UC05 |Excluir reserva |Essencial |
|UC06 |Consultar espaços | Essencial |
|UC07 |Gerenciar administradores | Importante |
|UC08 |Aprovar reserva | Importante|
|UC09 |Consultar Perguntas Frequentes | Desejável |
|UC10 |Gerar Relatório | Desejável |

# 5. Visão Lógica

## 5.1. Visão Geral

O sistema será desenvolvido em Django, que possui como padrão de desenvolvimento o MTV. Este se enquadra na arquitetura MVC, de acordo com o "The Django Book". Porém, a arquitetura implementada no Django possui algumas singularidades. Abaixo está uma imagem das camadas da arquitetura utilizada no django e como elas se relacionam.

![Imagem - Visão Geral](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/arquitetura1.png)

Na arquitetura MVC, a camada de controle é responsável por receber e processar requisições, além de controlar que modelos e visões serão utilizadas. A visão interage com o usuário e os modelos são responsável pelas classes de domínio e faz interface com o banco de dados, alem de ler e escrever dados. 
Na arquitetura MTV utilizada em Django, a camada de modelos não se preocupa com o banco de dados, pois ele é trabalhado na própria framework, a camada de visão é uma camada lógica, porém as requisições são tratadas também pelo próprio Django e a interface com o usuário é feita pela template.
Assim, nota-se que existem adaptações do Django em relação a arquitetura MVC, mas a comunicação entre as camadas e as suas diversas características e funções ainda enquadram o MTV como uma arquitetura MVC.  
## 5.2. Pacotes de Design Significativos do Ponto de Vista da Arquitetura
![Diagrama de Pacotes](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/DiagramaPacote.png)



Os pacotes de design signficativos são: models, templates, views, tests, factories e features. 

* model: faz interface com o banco de dados, é responsável por leitura, validação e escrita de dados.
* view: contém a camada lógica do sistema.
* template: faz interface com o usuário, contém as páginas HTML.
* tests: contém os testes unitários feitos no sistema.
* features: contém os testes de aceitação feitos no sistema.
* factories: contém as fábricas de objetos do sistema.


Nosso sistema foi criado em base de duas aplicações principais: user (usuário) e booking(reserva).

  
# 6. Visão da Implementação  

## 6.1. Visão Geral
![Imagem - Visão Geral](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/Diagrama_de_classe_soatributos.png)

## 6.2. Em Camadas

### Model

![Imagem - Model](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/Diagrama_de_classe_model.png)

### View

![Imagem - View](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/Diagrama_de_classe_view.png)

### Forms
![Imagem - Forms](https://raw.githubusercontent.com/wiki/fga-gpp-mds/2016.2-Time05-SalasFGA/img/Diagrama_de_classe_form.png)

# 7. Qualidade

A arquitetura utilizada no sistema afeta diretamente sua capacidade de manutenção, facilitando-a, já que sua implementação estará devidamente organizada. Além disso, como o MVC é um padrão de arquitetura amplamente utilizado, há efeitos práticos em sua confiabilidade.

# Referências

* [The Django Book](http://www.djangobook.com/en/2.0/). Acesso em 28/08/2016.