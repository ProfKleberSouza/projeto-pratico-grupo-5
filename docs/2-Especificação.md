# Especificações Do Projeto

<span style="color:red">Pré-requisitos: <a href="1-Contexto.md"> Documentação de Contexto</a></span>

> Apresente uma visão geral do que será abordado nesta parte do
> documento, enumerando as técnicas e/ou ferramentas utilizadas para
> realizar a especificações do projeto

## Personas
|Id        | Persona                                                            |
|----------|--------------------------------------------------------------------|
| ***1***  | Ernesto tem 21 anos, está cursando Sistemas de Informação e atua na área como desenvolvedor de sistemas para arcar com os custos da faculdade. Diante do cenário de pandemia, com o isolamento social e a pressão por conta do emprego e da faculdade, Ernesto tem desenvolvido alguns sintomas de ansiedade e passou a ver a necessidade de conversar com um psicológo.|
| ***2***  | Ana Clara tem 13 anos, está no 8º ano do ensino fundamental e é constantemente vítima de bullying de seus colegas de classe, além de não conseguir dialogar com seus pais o que vem gerando um grave quadro de depressão que necessita de atenção médica.|
|  ***3*** | Roberto é recém formado em psicologia e sempre teve atenção para causas sociais, agora com seu diploma ele vê a oportunidade de prestar ajuda profissional a pessoas que necessitam de atendimento psicológico mas não tem condição financeira para arcar com os custos de uma consulta. Roberto está buscando alguma ONG que o possibilite fazer alguns atendimentos de forma gratuita.|

> Enumere e detalhe as personas da sua solução. Para
> tanto, baseie-se tanto nos documentos disponibilizados na disciplina
> e/ou nos seguintes links:
>
> **Links Úteis**:
> - [Rock Content](https://rockcontent.com/blog/personas/)
> - [Hotmart](https://blog.hotmart.com/pt-br/como-criar-persona-negocio/)
> - [O que é persona?](https://resultadosdigitais.com.br/blog/persona-o-que-e/)
> - [Persona x Público-alvo](https://flammo.com.br/blog/persona-e-publico-alvo-qual-a-diferenca/)
> - [Mapa de Empatia](https://resultadosdigitais.com.br/blog/mapa-da-empatia/)
> - [Mapa de Stalkeholders](https://www.racecomunicacao.com.br/blog/como-fazer-o-mapeamento-de-stakeholders/)
>
> Lembre-se que você deve ser enumerar e descrever precisamente e
> personalizada todos os clientes ideais que sua solução almeja.

## Histórias de Usuários

Com base na análise das personas forma identificadas as seguintes histórias de usuários:

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Usuário     |Me autenticar pelo sistema, as funcionalidades do sistema se tornam disponíveis após a autenticação via login e senha registrados                 | Acessar as funcionalidades do sistema |
|Usuário       | Alterar minha senha dentro do sistema e fora, podendo apenas alterá-la por confirmação de e-mail A senha é uma sequência de caracteres que deve conter letras e números, obrigatoriamente                | Controle das minhas credencias no sistema|
|Administrador |Criar, remover e editar contas de secretários(as), para isso, visualizo uma lista de contas cadastradas contendo nome, e-mail, status e CRP, podendo filtrá-las pelo nome e também posso ordenar por data de criação e ordem alfabética         | Permitir o controle sobre as contas dos secretários(as)|
|Administrador|Criar, remover e editar contas de psicólogos(as), para isso, visualizo uma lista de contas cadastradas contendo nome, e-mail, status e CPF, podendo filtrá-las pelo nome ou por e-mail e também posso ordenar por data de criação, ordem alfabética e por quantidade de horários vagos abertos no mês ou semana| Permitir o controle sobre as contas dos psicólogos(as)|
|Secretário(a) |Visualizar os dados de quantidade de horários vagos que ainda estão disponíveis no mês e na semana. Também posso visualizar a quantidade de registros pendentes, reprovados e aprovados de psicólogos(as) cadastrados e dos membros da comunidade, após me autenticar no sistema  | Obter controle da situação a partir dos dados|
|Secretário(a)|Visualizar os dados de quantidade de horários vagos que ainda estão disponíveis no mês e na semana. Também posso visualizar a quantidade de registros pendentes, reprovados e aprovados de psicólogos(as) cadastrados e dos membros da comunidade |Obter controle da situação a partir dos dados.|
|Secretário(a)|Alterar o status das contas de psicólogos(as), esses status são definidos como aprovado, reprovado e pendente, para isso visualizo uma lista de psicólogos(as) contendo nome, e-mail, status e CRP, podendo filtrá-los pelo nome e status e também posso ordenar por data de criação, ordem alfabética e por quantidade de horários vagos abertos no mês ou semana. Caso necessite alterar o status ou visualizar mais dados da pessoa, posso acessar uma tela separada contendo todas as informações necessárias. |Gerenciar e visualizar as contas de psicólogos(as) cadastrados.|
|Secretário(a)|Alterar o status das contas dos membros da comunidade, esses status são definidos como aprovado, reprovado e pendente, para isso visualizo uma lista dos membros da comunidade contendo nome, e-mail, status e CPF, podendo filtrá-los pelo nome e status e também posso ordenar por data de criação e ordem alfabética. Caso necessite alterar o status ou visualizar mais dados da pessoa, posso acessar uma tela separada contendo todas as informações necessárias. |Gerenciar e visualizar as contas dos membros da comunidade cadastrados|
|Secretário(a) |Alocar paciente a um horário de um(a) psicólogos(as), para isso posso visualizar o calendário e a quantidade de profissionais disponíveis para aquele dia, caso eu acesse a data posso ver a lista dos profissionais aprovados e os horários de atendimento disponível, selecionando um profissional posso visualizar a lista de pacientes aprovados e realizar o agendamento da consulta. Após o agendamento é possível selecionar a funcionalidade de envio de e-mail para o profissional e o cliente com os detalhes da consulta.         |Permitir criar agendamentos de consultas e assim preencher os horários disponíveis dos psicólogos(as) para atendimento dos pacientes |
|Psicólogo(a) |Me cadastrar no sistema informando nome, telefone, email, CRP, Formado ou previsão de formatura, bairro, horários disponíveis de atendimento, interesse, por onde conheceu o trabalho da ASTLA, sugestão de comentário, após cadastrado meu status de cadastro é tido como pendente |Obter acesso ao sistema e participar nos serviços que a ONG oferece |
|Psicólogo(a) |Alterar todos os meus dados com exceção de nome, e-mail e CRP |Manter controle sobre os meus dados|
|Psicólogo(a) |Visualizar o status da minha conta, caso seja aprovado tenho acesso as funcionalidades do sistema. Caso seja reprovado eu consigo visualizar uma tela contendo informações de contato para regularizar minha situação |Obter o feedback do status do meu cadastro no sistema |
|Psicólogo(a) |Visualizar minha lista de horários marcados e pendentes, em outra tela posso visualizar os detalhes do paciente que irei atender e o histórico de atendimento dele |Manter controle sobre minha agenda e visualizar o laudo dos atendimentos anteriores do paciente |
|Membro da Comunidade|Me cadastrar no sistema da ONG, informando meus dados. Caso tenha uma limitação de horários, posso informá-los para ser atendido quando tiver disponibilidade|Obter acesso ao sistema e poder receber atendimento psicológico |
|Membro da Comunidade|Posso visualizar o status da minha conta, caso seja aprovado tenho acesso as funcionalidades do sistema. Caso seja reprovado eu consigo visualizar uma tela contendo informações de contato|Obter o feedback do status da minha conta, se estou ou não aprovado para receber auxílio de algum profissional |
|Membro da Comunidade|Visualizar minha lista de horários marcados no sistema|Controlar minha agenda e visualizar minhas consultas marcadas.|




> Apresente aqui as histórias de usuário que são relevantes para o
> projeto de sua solução. As Histórias de Usuário consistem em uma
> ferramenta poderosa para a compreensão e elicitação dos requisitos
> funcionais e não funcionais da sua aplicação. Se possível, agrupe as
> histórias de usuário por contexto, para facilitar consultas
> recorrentes à essa parte do documento.
>
> **Links Úteis**:
> - [Histórias de usuários com exemplos e template](https://www.atlassian.com/br/agile/project-management/user-stories)
> - [Como escrever boas histórias de usuário (User Stories)](https://medium.com/vertice/como-escrever-boas-users-stories-hist%C3%B3rias-de-usu%C3%A1rios-b29c75043fac)

## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto.

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| Permitir que o usuário cadastre tarefas | ALTA | 
|RF-002| Emitir um relatório de tarefas no mês   | MÉDIA |


### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| O sistema deve ser compatível com dispositivos móveis (*Android e iOS*) | MÉDIA | 
|RNF-002| O sistema deve possuir uma versão *Web* compatível com os navegadores de internet Google Chrome, Firefox, Safari e Mircrosoft Edge  |  MÉDIA | 
|RNF-003| O sistema deve processar requisições do usuário em no máximo 3s |  MÉDIA | 
|RNF-004| O sistema deve possuir uma interface com boa usabilidade, de fácil utilização |  MÉDIA | 
|RNF-005| O sistema deve promover fácil aprendizado em sua utilização |  MÉDIA | 
|RNF-006| O sistema deve possuir boa manutenibilidade, tal qual possibilite reparos e evoluções futuras      |  BAIXA | 
|RNF-007| O sistema deve operar com alta taxa de disponibilidade, acima de 95%      |  ALTA | 
|RNF-008| O sistema deverá atender às normas legais da Lei Geral de Proteção dos Dados (LGPD)         |  ALTA | 
|RNF-009| O sistema deve permitir que somente o perfil de Administrador efetue alterações e configurações dos demais perfis existentes  |  BAIXA | 
|RNF-010| O sistema deve exigir a autenticação de seus respectivos usuários para ser utilizado |  BAIXA | 
|RNF-011| Os dispositivos móveis (*Smartphones*) devem possuir no mínimo um processador com dois núcleos físicos, 2GB de memória RAM e 4GB de armazenamento interno       |  BAIXA | 
|RNF-012| O sistema deve efetuar a comunicação e tranporte de informações através do protocolo *Hypertext Transfer Protocol* (HTTP)         |  BAIXA | 
|RNF-013| O sistema deve ser submetido a testes de unidade, integração e aceitação       |  BAIXA | 
|RNF-014| A versão do sistema compatível com dispositivos móveis deve ser desenvolvida utilizando o *framework* Flutter, da linguagem de programação Dart     |  MÉDIA | 
|RNF-015| A versão *Web* do sistema deve ser desenvolvida utilizando o *framework* Angular, da linguagem de programação Javascript        |  MÉDIA | 
|RNF-016| O sistema deve possuir uma API, a qual deve ser desenvolvida utilizando o *framework* .Net Core, da linguagem de programação C#         |  MÉDIA | 
|RNF-017| O sistema deve utilizar o banco de dados relacional Microsoft SQL Server        |  BAIXA | 


> Com base nas Histórias de Usuário, enumere os requisitos da sua
> solução. Classifique esses requisitos em dois grupos:
>
> - [Requisitos Funcionais
>   (RF)](https://pt.wikipedia.org/wiki/Requisito_funcional):
>   correspondem a uma funcionalidade que deve estar presente na
>   plataforma (ex: cadastro de usuário).
>
> - [Requisitos Não Funcionais
>   (RNF)](https://pt.wikipedia.org/wiki/Requisito_n%C3%A3o_funcional):
>   correspondem a uma característica técnica, seja de usabilidade,
>   desempenho, confiabilidade, segurança ou outro (ex: suporte a
>   dispositivos iOS e Android).
>
> Lembre-se que cada requisito deve corresponder à uma e somente uma
> característica alvo da sua solução. Além disso, certifique-se de que
> todos os aspectos capturados nas Histórias de Usuário foram cobertos.

## Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01| O projeto deverá ser entregue até o final do semestre letivo |
|02| O projeto se limita a atender todos os requisitos funcionais, requisitos não funcionais e funcionalidades especificadas neste documento |


> Enumere as restrições à sua solução. Lembre-se de que as restrições
> geralmente limitam a solução candidata.
> 
> **Links Úteis**:
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)
