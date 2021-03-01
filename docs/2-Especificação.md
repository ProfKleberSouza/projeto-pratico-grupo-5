# Especificações Do Projeto

<span style="color:red">Pré-requisitos: <a href="1-Contexto.md"> Documentação de Contexto</a></span>

## Personas
|Id        | Persona                                                            |
|----------|--------------------------------------------------------------------|
| ***1***  | Ernesto tem 21 anos, está cursando Sistemas de Informação e atua na área como desenvolvedor de sistemas para arcar com os custos da faculdade. Diante do cenário de pandemia, com o isolamento social e a pressão por conta do emprego e da faculdade, Ernesto tem desenvolvido alguns sintomas de ansiedade e passou a ver a necessidade de conversar com um psicológo.|
| ***2***  | Ana Clara tem 13 anos, está no 8º ano do ensino fundamental e é constantemente vítima de bullying de seus colegas de classe, além de não conseguir dialogar com seus pais o que vem gerando um grave quadro de depressão que necessita de atenção médica.|
|  ***3*** | Roberto é recém formado em psicologia e sempre teve atenção para causas sociais, agora com seu diploma ele vê a oportunidade de prestar ajuda profissional a pessoas que necessitam de atendimento psicológico mas não tem condição financeira para arcar com os custos de uma consulta. Roberto está buscando alguma ONG que o possibilite fazer alguns atendimentos de forma gratuita.|
|  ***4*** | Paula é gerente uma ONG que atende membros da comunidade de forma gratuita  |

## Histórias de Usuários

Com base na análise das personas forma identificadas as seguintes histórias de usuários:

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Usuário     |Me autenticar pelo sistema, as funcionalidades do sistema se tornam disponíveis após a autenticação via login e senha registrados                 | Acessar as funcionalidades do sistema |
|Usuário       | Alterar minha senha dentro do sistema e fora, podendo apenas alterá-la por confirmação de e-mail A senha é uma sequência de caracteres que deve conter letras e números, obrigatoriamente                | Controle das minhas credencias no sistema|
|Administrador |Criar, remover e editar contas de secretários(as), para isso, visualizo uma lista de contas cadastradas contendo nome, e-mail, status e CRP, podendo filtrá-las pelo nome e também posso ordenar por data de criação e ordem alfabética         | Permitir o controle sobre as contas dos secretários(as)|
|Administrador|Criar, remover e editar contas de psicólogos(as), para isso, visualizo uma lista de contas cadastradas contendo nome, e-mail, status e CPF, podendo filtrá-las pelo nome ou por e-mail e também posso ordenar por data de criação, ordem alfabética e por quantidade de horários vagos abertos no mês ou semana| Permitir o controle sobre as contas dos psicólogos(as)|
|Secretário(a)|Visualizar relatório dos dados de quantidade de horários vagos que ainda estão disponíveis no mês e na semana. Também posso visualizar a quantidade de registros pendentes, reprovados e aprovados de psicólogos(as) cadastrados e dos membros da comunidade |Obter controle da situação a partir dos dados.|
|Secretário(a)|Alterar o status das contas de psicólogos(as), esses status são definidos como aprovado, reprovado e pendente, para isso visualizo uma lista de psicólogos(as) contendo nome, e-mail, status e CRP, podendo filtrá-los pelo nome e status e também posso ordenar por data de criação, ordem alfabética e por quantidade de horários vagos abertos no mês ou semana. Caso necessite alterar o status ou visualizar mais dados da pessoa, posso acessar uma tela separada contendo todas as informações necessárias. |Gerenciar e visualizar as contas de psicólogos(as) cadastrados.|
|Secretário(a)|Alterar o status das contas dos membros da comunidade, esses status são definidos como aprovado, reprovado e pendente, para isso visualizo uma lista dos membros da comunidade contendo nome, e-mail, status e CPF, podendo filtrá-los pelo nome e status e também posso ordenar por data de criação e ordem alfabética. Caso necessite alterar o status ou visualizar mais dados da pessoa, posso acessar uma tela separada contendo todas as informações necessárias. |Gerenciar e visualizar as contas dos membros da comunidade cadastrados|
|Secretário(a) |Alocar paciente a um horário de um(a) psicólogos(as), para isso posso visualizar o calendário e a quantidade de profissionais disponíveis para aquele dia, caso eu acesse a data posso ver a lista dos profissionais aprovados e os horários de atendimento disponível, selecionando um profissional posso visualizar a lista de pacientes aprovados e realizar o agendamento da consulta. Após o agendamento é possível selecionar a funcionalidade de envio de e-mail para o profissional e o cliente com os detalhes da consulta.         |Permitir criar agendamentos de consultas e assim preencher os horários disponíveis dos psicólogos(as) para atendimento dos pacientes |
|Psicólogo(a) |Me cadastrar no sistema informando nome, telefone, email, CRP, Formado ou previsão de formatura, bairro, horários disponíveis de atendimento, interesse, por onde conheceu o trabalho da ASTLA, sugestão de comentário, após cadastrado meu status de cadastro é tido como pendente |Obter acesso ao sistema e participar nos serviços que a ONG oferece |
|Psicólogo(a) |Alterar todos os meus dados com exceção de nome, e-mail e CRP |Manter controle sobre os meus dados|
|Psicólogo(a) |Visualizar o status da minha conta, caso seja aprovado tenho acesso as funcionalidades do sistema. Caso seja reprovado eu consigo visualizar uma tela contendo informações de contato para regularizar minha situação |Obter o feedback do status do meu cadastro no sistema |
|Psicólogo(a) |Visualizar minha lista de horários marcados e pendentes, em outra tela posso visualizar os detalhes do paciente que irei atender e o histórico de atendimento dele |Manter controle sobre minha agenda e visualizar o laudo dos atendimentos anteriores do paciente |
|Membro da Comunidade|Me cadastrar no sistema da ONG, informando meus dados. Caso tenha uma limitação de horários, posso informá-los para ser atendido quando tiver disponibilidade|Obter acesso ao sistema e poder receber atendimento psicológico |
|Membro da Comunidade|Posso visualizar o status da minha conta, caso seja aprovado tenho acesso as funcionalidades do sistema. Caso seja reprovado eu consigo visualizar uma tela contendo informações de contato|Obter o feedback do status da minha conta, se estou ou não aprovado para receber auxílio de algum profissional |
|Membro da Comunidade|Visualizar minha lista de horários marcados no sistema|Controlar minha agenda e visualizar minhas consultas marcadas|


## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto.

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| Permitir que o usuario cadastre-se no sistema como paciente ou psicólogo | ALTA | 
|RF-002| Permitir ao usuário autenticar-se no sistema informando email e senha | ALTA |
|RF-003| Permitir ao psicólogo especificar quais são seus horários de disponibilidade   | MÉDIA |
|RF-004| Permitir ao secretário alocar consultas entre pacientes e psicólogos aprovados   | ALTA |
|RF-005| Permitir ao usuário alterar sua senha por confirmação de email   | BAIXA |
|RF-006| Permitir ao administrador criar, alterar e excluir contas de secretário(a)  | MÉDIA |
|RF-007| Permitir ao secretário visualizar a quantidade de horários vagos disponíveis do mês ou semana corrente   | MÉDIA |
|RF-008| Permitir ao secretário visualizar um relatório dos registros de psicólogo e paciente   | BAIXA |
|RF-009| Permitir ao secretário visualizar uma listagem com os dados e situação da conta de psicólogos e pacientes   | ALTA |
|RF-010| Permitir ao secretário filtrar pelo nome e status a listagem de psicólogos e pacientes   | MÉDIA |
|RF-011| Permitir ao secretário alterar o status das contas de psicólogos e pacientes para aprovado ou reprovado   | ALTA |
|RF-012| Permitir ao secretário ordenar a listagem de psicólogos e pacientes pela data de criação, nome e quantidade de horários de vagos abertos no mês ou semana   | MÉDIA |
|RF-013| Permitir ao visualizar de forma detalhada os dados de psicólogos e pacientes   | ALTA |
|RF-014| Permitir ao visualizar de forma detalhada os dados de psicólogos e pacientes   | ALTA |


### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| O sistema deve ser responsivo para rodar em um dispositivos móvel | MÉDIA | 
|RNF-002| Deve processar requisições do usuário em no máximo 3s |  BAIXA | 

## Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01| O projeto deverá ser entregue até o final do semestre letivo |
|02| O projeto se limita a atender todos os requisitos funcionais, requisitos não funcionais e funcionalidades especificadas neste documento |
