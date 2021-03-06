[retornar para Especificações de Caso de Uso](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/wiki/Especifica%C3%A7%C3%A3o-de-Casos-de-Uso)

#1. Descrição

Permite que usuários cadastrados excluam reservas de espaços.

#2. Ator

Corpo Acadêmico:exclui reservas feitas em seu nome.

Administrador: pode excluir qualquer reserva.

#3. Pré condição

O usuário deve estar logado.

#4. Pós condição

A reserva será excluída.

#5. Fluxo Principal

[FP01] O caso de uso se inicia quando o usuário seleciona a opção de “Minhas Reservas” na barra de menu.

[FP02] O sistema encaminha o usuário para a página de reservas e lista todas as reservas do usuário.

[FP03] O usuário aperta no botão "x", da reserva que deseja deletar, para enviar a solicitação. 

[FP04] O usuário clica em "Confirmar".

[FP05] O sistema exclui a reserva e exibe uma mensagem para o usuário.


#6. Fluxo de Alternativo

[FA01] O administrador exclui uma reserva de outro usuário.

[FA01.1] O administrador clica na opção de pesquisar usuários.

[FA01.2] O administrador insere o nome do usuário que deseja pesquisar.

[FA01.3] O administrador seleciona o usuário que deseja ver.

[FA01.4] O administrador seleciona seleciona a opção "visualizar reservas"

[FA01.5] O administrador é encaminhado para o [FP02] do "Excluir Reserva".


[FA02] Após o passo 2 do fluxo principal [FP02] o usuário queira encontrar a reserva que deseja excluir por nome da reserva e/ou data da reserva, ele preenche ao menos um desses campos, retorna para [FP03]

[FA03] A partir do [FA01], o administrador pesquisa uma reserva.

[FA03.1] O administrador seleciona a reserva que deseja excluir.

[FA03.2] O administrador é encaminhado para o [FP03].


[FA04] A partir do [FA01], o administrador pesquisa um espaço.

[FA04.1] O administrador consulta as reservas daquele espaço.

[FA04.2] O administrador seleciona a reserva que deseja excluir.

[FA04.3] O administrador é encaminhado para o [FP03].

#7. Fluxo de Exceção

[FE01] No passo 4 do fluxo principal [FP04] o usuário aperta no botão "cancelar" , retorna para [FP02].

[FE02] No passo 2 do [FA01] o administrador digita o nome de um usuário que não existe, retorna para [FA01] sinalizando que o usuário digitado não existe.

[FE03] No [FA02] o usuário digita o nome de uma reserva e/ou a data de uma reserva que ele não possui, retorna para [FP02] sinalizando que não existe reserva com esse nome e/ou data.


[retornar para Especificações de Caso de Uso](https://github.com/fga-gpp-mds/2016.2-SAS_FGA/wiki/Especifica%C3%A7%C3%A3o-de-Casos-de-Uso)