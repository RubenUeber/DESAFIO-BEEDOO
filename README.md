## Desafio Beedoo - Projeto de Teste de Software do Módulo de Cursos :bulb:

:link: Links: <br/>
Link de cenários de testes: https://docs.google.com/spreadsheets/d/1oNtuyJdK5_X61uXFoT58DhfogsZzxXSi/edit?usp=sharing&ouid=101283374288346856276&rtpof=true&sd=true 
<br/> Link com bugs cadastrados: https://docs.google.com/spreadsheets/d/1xrT8dowAzgPlRit_IwqtZURaN-4l4aKFDlzgp2Kja08/edit?usp=sharing
<br/> Link evidências do teste em formato MP4: https://drive.google.com/drive/folders/1kjOJ0WHs6y3x0XYleWdPdFZVxt4Hv5Bj?usp=sharing

<br/> **Considerações iniciais**:
<br/>
<br/> :bug: No relatório de bugs foi utilizado a metodologia tradicional de bug report, pois para o caso concreto comunicam melhor e com mais objetividade as inconsistências por conter os seguintes atributos:
<br/> ID do Bug
<br/> Data
<br/> Status
<br/> Prioridade
<br/> Severidade
<br/> Afetado pelo bug
<br/> Título do bug
<br/> Descrição do bug
<br/> Passo para reprodução
<br/> E outras informações importantes.

### Visão Geral
Este projeto tem o objetivo de realizar testes de software do Módulo de Cursos em vistas a garantir a qualidade e a robustez da plataforma de aprendizado online da empresa. Tendo em vista ser este um módulo importante do projeto, é essencial que a sua funcionalidade e usabilidade facilitem o processo de aprendizado do usuário. Através deste projeto de teste, procurei elaborar user stories sob a pespectiva do usuário e que reflissem sua real necessidade e, a partir daí, validar cenários de testes de fluxo principal e de excessão, abordando a jornada do usuário e visando mitigar inconsistências.

### Decisão tomada para criar user story

A decisão para criar as user stories a seguir partiu de boas práticas do desenvolvimento ágil, levando em consideração o ponto de vista do usuário, seus objetivos, estruturada de forma não técnica para traduzir o mais próximo possível a jornada do usuário e dar contexto mais assertivo na hora do desenvolvimento do software, no caso, a plataforma de cursos da Beedoo.
Cada user story revela um pedaço da plataforma de cursos da Beedoo onde o usuário interage com as funcionalidades. Além disso, as user stories foram estruturadas no seguinte formato: 
- Como usuário [persona]: para quem estamos criando a feature
- Gostaria [intenção]: demostra a intenção do usuário, o que ela quer alcançar
- Assim [vontade]: demostra o que a persona pretende alcançar como resultado esperado <br/> <br/>
Sendo considerado boa prática no contexto ágil, procurei manter o foco no usuário com os seguintes perfils: <br/> <br/>
- Perfil de funcionário da empresa que contratou a plataforma da Beedoo, contextualizando as várias interações que este usuário irá ter com a aplicação;
- Perfil de gestor desta empresa, contextualizando as interações que este usuário irá ter com a aplicação, tais como cadastrar cursos, editar cursos, excluir cursos, fazer login, etc;
- Perfil de cliente extrangeiro (EUA/Europa);
- Perfil de usuário geral da plataforma e suas diversas interações.


### User stories

**1º User story: Cadastrar curso**
  
Como usuário da plataforma BeeDoo e gestor da empresa A <br/>
Gostaria de poder acessar a aba "CADASTRAR CURSO" da plataforma <br/>
Assim posso preencher o formulário e cadastrar cursos para meus funcionários <br/>

Critérios de aceite:
- Ao clicar na aba "CADASTRAR CURSO", o formulário deve ser exibido para o usuário
- A aplicação deve permitir o preenchimento dos dados do curso no formulário
- Ao clicar no botão "CADASTRAR CURSO", a aplicação deve redirecionar para a página de Listar Cursos e exibir o curso cadastrado
- Após o cadastro do curso, a aplicação deverá exibir um popup informando que o curso foi cadastrado com sucesso

**2º User story: Visualizar lista de cursos**
  
Como usuário gestor da empresa A <br/>
Gostaria de poder acessar a aba "LISTAR CURSOS" <br/>
Assim posso visualizar o painel de lista de cursos cadastrados <br/>

Critérios de aceite:
- Ao clicar na aba "LISTAR CURSOS", o usuário deve ser redirecionado para o módulo que clicou
- A aplicação deve exibir a lista de cursos cadastrados com todos os detalhes

**3º User story: Exclusão de cursos**
  
Como usuário gestor da empresa A <br/>
Gostaria de poder excluir um curso cadastrado na aba "LISTAR CURSOS" <br/>
Assim posso excluir um curso que não é mais necessário que seja exibido para o funcionário <br/>

Critérios de aceite:
- Ao clicar em "Excluir curso", o card do curso deverá ser excluido com sucesso

### **Outras user stories complementares para a feature desenvolvida no contexto ágil** 

**4º User story: Cadastro de usuário**
  
Como usuário gestor da empresa A <br/>
Gostaria de poder realizar o cadastro do meu usuário na plataforma Beedoo <br/>
Assim posso acessar a plataforma e usufruir dos benefícios <br/>

Critérios de aceite:
- A aplicação deve exibir uma aba apenas para cadastro do usuário
- Ao preencher o formulário de cadastro, a aplicação deve enviar um e-mail de confirmação de cadastro ao usuário

**5º User story: Login de usuário**
  
Como usuário gestor da empresa A <br/>
Gostaria de poder realizar login na plataforma Beedoo <br/>
Assim posso acessar os paineis disponíveis para fazer a gestão de aprendizado dos meus funcionários <br/>

Critérios de aceite:
- A aplicação deve exibir uma tela de login 
- A tela de login deve exibir os campos de login e senha
- A tela de login deve exibir link de redefinição de senha
- Ao digitar o login incorreto, a aplicação deve informar que o usuário digitou um login inválido
- Ao digitar a senha incorreta, a aplicação deve informar que a senha digitada está inválida
- Ao digitar o login e as credenciais corretas, a aplicação deverá permitir o login com sucesso

**6º User story: Login de usuário funcionário**
  
Como usuário funcionário da empresa A <br/>
Gostaria de poder realizar login na plataforma BeeDoo <br/>
Assim posso acessar a plataforma e realizar os cursos oferecidos pela empresa <br/>

Critérios de aceite:
- A aplicação deve exibir uma tela de login 
- A tela de login deve exibir os campos de login e senha
- A tela de login deve exibir link de redefinição de senha
- Ao digitar o login incorreto, a aplicação deve informar que o usuário digitou um login inválido
- Ao digitar a senha incorreta, a aplicação deve informar que a senha digitada está inválida
- Ao digitar o login e as credenciais corretas, a aplicação deverá permitir o login com sucesso

**7º User story: Acesso a curso**
  
Como usuário funcionário da empresa A <br/>
Gostaria de poder realizar o acesso ao curso cadastrado na plataforma BeeDoo <br/>
Assim posso acessar e atender ao curso oferecido pela empresa <br/>

Critérios de aceite:
- Ao clicar no curso exibido na tela, a aplicação deve exibir o curso selecionado

**8º User story: Acesso à plataforma BeeDoo (perfis de usuário)** 
  
Como usuário da empresa A <br/>
Gostaria de poder escolher o meu perfil de acesso no login da plataforma BeeDoo <br/>
Assim posso acessar com perfil de gestor ou de funcionário <br/>

Critérios de aceite:
- Ao acessar o módulo de login da plataforma, a aplicação deve exibir a opção de logar com perfil de gestor ou de funcionário
- Ao logar com perfil de gestor, a aplicação deve exibir a opção de criar cursos e outras features como exibição de estatísticas dos funcionários
- Ao logar com perfil de funcionário, a aplicação deve exibir os cursos e outros atributos relacionados ao perfil de funcionário

**9º User story: Visualização do card do curso** 
  
Como usuário da empresa A <br/>
Gostaria de poder visualizar o card com as informações importantes sobre o curso <br/>
Assim posso verificar qual curso melhor se adequa às necessidades do momento na empresa <br/>

Critérios de aceite:
- Ao acessar a plataforma, o usuário deve visualizar os cursos disponíveis e todas as seções de recomendações e dashboard

**10º User story: Retornar à página inicial da plataforma** 
  
Como usuário da empresa A <br/>
Gostaria de poder retornar à página inicial da plataforma <br/>
Assim posso visualizar a página inicial <br/>

Critérios de aceite:
- A aplicação deve exibir um botão de back nas páginas de navegação
- Ao clicar no botão de back, a aplicação deve retornar uma página 

**11º User story: Efetuar logout da plataforma**
  
Como usuário da empresa A <br/>
Gostaria de poder efetuar o logout da plataforma <br/>
Assim posso sair da plataforma <br/>

Critérios de aceite:
- A aplicação deve exibir um botão de logout no header
- Ao clicar no botão de logout, o usuário deve sair da aplicação e ser redirecionado para a tela de login

**12º User story: Editar curso**
  
Como usuário gestor da empresa A <br/>
Gostaria de poder editar o curso cadastrado <br/>
Assim posso editar o curso conforme necessidade e demanda <br/>

Critérios de aceite:
- A aplicação deve exibir no card do curso uma opção de edição do curso
- Ao clicar na opção de edição, o usuário deverá poder editar o curso selecionado para edição
- Após editar o curso, a aplicação deverá exibir as alterações realizadas

**13º User story: Compartilhar curso com colega**
  
Como usuário funcionário da empresa A <br/>
Gostaria de poder ter um botão de compartilhamento do curso <br/>
Assim posso compartilhar o curso/conteúdo com um colega <br/>

Critérios de aceite:
- A aplicação deverá exibir uma opção de compartilhamento de conteúdo/curso com terceiros
- Após o usuário clicar no ícone de compartilhamento, a aplicação deverá exibir a opção de enviar para um amigo

**14º User story: Retorno visual dos botões**
  
Como usuário da plataforma BeeDoo <br/>
Gostaria de poder ter o retorno visual de mouse hover e da ação de clicar nos botões da plataforma <br/>
Assim posso entender que minha ação foi registrada e a aplicação responde conforme esperado <br/>

Critérios de aceite:
- Ao passar o mouse em cima dos botões, os mesmos devem mudar de cor
- Ao clicar nos botões, os mesmos devem mostrar um indicador de carregamento
- Ao retirar a seta do mouse de cima do botão, o mesmo deve retornar a cor estática anterior

**15º User story: Acessibilidade da plataforma**
  
Como usuário deficiente visual da plataforma BeeDoo <br/>
Gostaria de poder acessar os links úteis a partir do teclado e com recurso de audiodescrição <br/>
Assim posso entender e ser suficientemente capaz de navegar pela plataforma sem problemas <br/>

Critérios de aceite:
- A plataforma deve ter uma opção de acionamento de acessibilidade
- A plataforma deve permitir ser navegada através do teclado do computador
- A plataforma deve ter o recurso de audiodescrição

**16º User story: Acessibilidade da plataforma Surdos**
  
Como usuário portador de deficiência auditiva <br/>
Gostaria de poder acessar o recurso de tradução simultânea de libras na plataforma BeeDoo <br/>
Assim posso navegar na plataforma com tranquilidade e ter acesso aos cursos com tradução simultânea em libras <br/>

Critérios de aceite:
- A plataforma deve ter uma opção de acionamento de acessibilidade
- A plataforma deve permitir que o usuário clique nos textos e instantaneamente seja exibido a tradução em libras na tela
- Os conteúdos/cursos devem vir com a opção de tradução em libras
- Ao clicar no botão de acessibilidade na plataforma, o recurso deverá ser ocultado até que o usuário retome a ação

**17º User story: Filtragem de cursos cadastrados**
  
Como usuário da plataforma Beedoo <br/>
Gostaria de poder filtrar os cursos por categoria ou palavra-chave <br/>
Assim posso encontrar de maneira mais intuitiva um curso específico <br/>

Critérios de aceite:
- A plataforma deve ter uma opção de filtragem de cursos incluindo "categoria" e "palavra-chave"
- Ao inserir uma categoria ou palavra-chave, a aplicação deve trazer o resultado conforme o filtro selecionado
- Ao limpar o filtro, a aplicação deve trazer o resultado com filtros limpos

**18º User story: Confirmação de matricula de curso**
  
Como usuário da plataforma Beedoo <br/>
Gostaria de poder me matricular em um dos cursos oferecidos na plataforma e receber a confirmação <br/>
Assim posso acessar aquele curso que me matriculei e dar continuidade <br/>

Critérios de aceite:
- A plataforma deve ter a opção de matricula de curso
- O card do curso deve exibir se o usuário está matriculado naquele curso ou não
- Ao limpar o filtro, a aplicação deve trazer o resultado com filtros limpos

**19º User story: Opção de avaliar curso**
  
Como usuário da plataforma Beedoo <br/>
Gostaria de poder atribuir uma avaliação ao curso através de um botão <br/>
Assim posso demostrar meu interesse no curso <br/>

Critérios de aceite:
- O card do curso deve ter um botão para o usuário acionar
- O botão deve possuir uma numeração onde a cada vez clicado, aumenta um número
- Ao acionar o botão de "curtir", o número na lateral do icone deve aumentar +1
- O botão deve permitir apenas um clique por usuário
- Ao clicar novamente no botão, o número deve decrescer -1

**20º User story: Status do curso**
  
Como usuário da plataforma Beedoo <br/>
Gostaria de poder visualizar os cursos com o status de "A ser iniciado", "Em andamento" e "Concluído" <br/>
Assim consigo ver o status de todos os cursos na minha tela de maneira simples e rápida <br/>

Critérios de aceite:
- O curso que não estiver sido iniciado pelo usuário, deve ter uma tag com a descrição "A ser iniciado" e cor cinza
- O curso que estiver em andamento pelo usuário, deve ter uma tag com a descrição "Em andamento" e cor amarelo
- O curso que estiver na fase de concluído pelo usuário, deve ter uma tag com a descrição "Concluído" e cor verde

**21º User story: Seção dos curso com base no status**
  
Como usuário da plataforma Beedoo <br/>
Gostaria de poder visualizar os cursos em formato de seção na página de cursos, contendo os títulos de cada status: "A ser iniciado", "Em andamento" e "Concluído" <br/>
Assim consigo visualizar de maneira mais fácil os cursos disponíveis na página com base em seu status <br/>

Critérios de aceite:
- A plataforma deve exibir ao usuário 3 seções com o título "A ser iniciado", "Em andamento" e "Concluído", respectivamente
- O curso que não estiver sido iniciado pelo usuário, deve está na seção de "A ser iniciado" 
- O curso que estiver em andamento pelo usuário, deve está na seção de "Em andamento" 
- O curso que estiver na fase de concluído pelo usuário, deve está na seção de "Concluído"

**22º User story: Dashboard dos cursos**
  
Como usuário da plataforma Beedoo <br/>
Gostaria de poder visualizar um dashboard contendo informações em números com base no status de cada curso matriculado <br/>
Assim consigo visualizar de maneira resumida e rápida os cursos com base em seu status <br/>

Critérios de aceite:
- A plataforma deve exibir um dashboard com a informação de "Cursos aprovados", "Cursos reprovados", "Cursos em andamento", "Cursos concluídos", "Score geral"

**23º User story: Seção de recomendação de cursos**
  
Como usuário da plataforma Beedoo <br/>
Gostaria de poder visualizar uma seção na página dedicada a recomendar cursos/conteúdos com base no aprendizado de IA extraido a partir das minhas reações <br/>
Assim consigo me dedicar de maneira mais assertiva e otimizada a um curso/conteúdo de meu interesse <br/>

Critérios de aceite:
- A plataforma deve exibir uma seção com o título "Recomandações para você" com cursos recomendados
- Os cursos recomendados devem ser baseados nas reações que o usuário tem dentro da plataforma
- As reações devem ser coletadas a partir da Inteligência Artificial dedicada

**24º User story: Página dedicada a estatísticas**
  
Como usuário da plataforma Beedoo e gestor da empresa XPTO <br/>
Gostaria de poder visualizar uma seção na página dedicada a recomendar cursos/conteúdos com base no aprendizado de IA extraido a partir das minhas reações <br/>
Assim consigo me dedicar de maneira mais assertiva e otimizada a um curso/conteúdo de meu interesse <br/>

Critérios de aceite:
- A plataforma deve exibir uma seção com o título "Recomandações para você" com cursos recomendados
- Os cursos recomendados devem ser baseados nas reações que o usuário tem dentro da plataforma
- As reações devem ser coletadas a partir da Inteligência Artificial dedicada

**25º User story: Página com opção de idioma inglês**
  
Como usuário de empresa extrangeira da pataforma Beedoo <br/>
Gostaria de poder alterar o idioma da plataforma para inglês <br/>
Assim consigo entender meu idioma nativo ao navegar na plataforma <br/>

Critérios de aceite:
- A plataforma deve exibir uma opção no header para ser possível a alteração de idioma da plataforma
- Ao clicar na opção de idioma "english", toda a plataforma deve ser alterada para o idioma selecionado
- Ao clicar na opção de idioma "português", toda a plataforma deve ser alterada para o idioma selecionado
- A alteração de idioma deve ser de forma instantânea para evitar que a experiência do usuário seja prejudicada

### Melhorias a serem implementada :computer:

|Melhorias|Feature|
| -------- | -------- |
|Implementar limite de caracteres no campo Nome do curso|Cadastro de curso|
|Implementar limite de caracteres no campo Descrição do curso|Cadastro de curso|
|Implementar limite de caracteres no campo Instrutor do curso|Cadastro de curso|
|Impedir que data FIM seja menor que data de INICIO no calendário|Cadastro de curso|
|Limitar valor limite a 0 no número de vagas do curso|Cadastro de curso|
|Implementar botão de editar curso|Listar cursos|
|Implementar seta de retorno para a página inicial|Cadastro de curso|
|Ajustar layout dos cursos da tela de "lista de cursos" para padronizar cards|Listar cursos|
|Implementar cadastro de usuário com perfils e acessos diferentes na plataforma|Cadastro de users|
|Implementar tela de login de usuário|Tela de login|
|Implementar botão de compartilhamento de curso|Lista de cursos|
|Implementar botão de avaliação de curso|Lista de cursos|
|Implementar tag de status do curso|Lista de cursos|
|Implementar acessibilidade de audiodescrição para cegos na plataforma|Toda plataforma|
|Implementar acessibilidade de libras para surdos na plataforma|Toda plataforma|
|Implementar seção dos curso com base no status|Lista de cursos|
|Implementar filtragem de cursos cadastrados dos curso com base no status|Lista de cursos|
|Implementar opção de idioma inglês|Toda plataforma|
|Implementar página dedicada a estatísticas|Estatística|
|Implementar seção de recomendação de cursos|Lista de cursos|
|Implementar dashboard dos cursos|Lista de cursos|
|Implementar confirmação de matricula de curso|Lista de cursos|
|Implementar controle de acesso aos usuários|Login|





