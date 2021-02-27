# Especificações Do Projeto

<span style="color:red">Pré-requisitos: <a href="1-Contexto.md"> Documentação de Contexto</a></span>

> Apresente uma visão geral do que será abordado nesta parte do
> documento, enumerando as técnicas e/ou ferramentas utilizadas para
> realizar a especificações do projeto

## Personas

***Exemplo-*** Pedro Paulo tem 26 anos, é arquiteto recém-formado e autônomo. Pensa em
se desenvolver profissionalmente através de um mestrado fora do país,
pois adora viajar, é solteiro e sempre quis fazer um intercâmbio. Está
buscando uma agência que o ajude a encontrar universidades na Europa
que aceitem alunos estrangeiros.

***1-*** Ernesto tem 21 anos, está cursando Sistemas de Informação e atua na área como desenvolvedor de sistemas para arcar com os custos da faculdade. Diante do cenário de pandemia, com o isolamento social e a pressão por conta do emprego e da faculdade, Ernesto tem desenvolvido alguns sintomas de ansiedade e passou a ver a necessidade de conversar com um psicológo.

***2-*** Ana Clara tem 13 anos, está no 8º ano do ensino fundamental e é constantemente vítima de bullying de seus colegas de classe, além de não conseguir dialogar com seus pais o que vem gerando um grave quadro de depressão que necessita de atenção médica.

***3-*** Roberto é recém formado em psicologia e sempre teve atenção para causas sociais, agora com seu diploma ele vê a oportunidade de prestar ajuda profissional a pessoas que necessitam de atendimento psicológico mas não tem condição financeira para arcar com os custos de uma consulta. Roberto está buscando alguma ONG que o possibilite fazer alguns atendimentos de forma gratuita.


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
|Administrador       | Me autenticar pelo sistema, as funcionalidades do sistema se tornam disponíveis após a autenticação via login e senha registrados                 | Acessar as funcionalidades do sistema |
|Administrador       | Alterar minha senha dentro do sistema e fora, podendo apenas alterá-la por confirmação de e-mail A senha é uma sequência de caracteres que deve conter letras e números, obrigatoriamente                | Alterar minha senha de acesso de forma segura| |
|Administrador       | Criar, remover e editar contas de secretários(as), para isso, visualizo uma lista de contas cadastradas, podendo filtrá-las pelo nome ou por e-mail e também posso ordenar por data de criação e ordem alfabética         | Permitir o controle sobre as contas dos secretários(as)|
|Administrador & Secretário(a)       | Criar, remover e editar contas de psicólogos(as), para isso, visualizo uma lista de contas cadastradas, podendo filtrá-las pelo nome ou por e-mail e também posso ordenar por data de criação, ordem alfabética e por quantidade de horários vagos abertos no mês ou semana         | Permitir o controle sobre as contas dos psicólogos(as)|
|Secretário(a)       |  Me autenticar pelo sistema, as funcionalidades do sistema se tornam disponíveis após a autenticação via e-mail e senha registrados        | Acessar as funcionalidades do sistema|
|Secretário(a)       | Alocar paciente a um horário de um(a) psicólogos(as), para isso posso visualizar o calendário e a quantidade de profissionais disponíveis para aquele dia, caso eu acesse a data posso ver a lista dos profissionais e os horários de atendimento disponível, selecionando um profissional posso visualizar a lista de pacientes e realizar o agendamento da consulta Após o agendamento é possível selecionar a funcionalidade de envio de e-mail para o profissional e o cliente com os detalhes da consulta         |Permitir criar agendamentos de consultas e assim preencher os horários disponíveis dos psicólogos(as) para atendimento dos pacientes |



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
|RNF-001| O sistema deve ser responsivo para rodar em um dispositivos móvel | MÉDIA | 
|RNF-002| Deve processar requisições do usuário em no máximo 3s |  BAIXA | 

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
|01| O projeto deverá ser entregue até o final do semestre |
|02| Não pode ser desenvolvido um módulo de backend        |


> Enumere as restrições à sua solução. Lembre-se de que as restrições
> geralmente limitam a solução candidata.
> 
> **Links Úteis**:
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)
