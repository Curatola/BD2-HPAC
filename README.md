# TRABALHO 01 : HPAC - Histórico de Pacientes
Trabalho de revisão desenvolvido no início da disciplina de BD2.

# Sumário

Histórico de Pacientes é um sistema de banco de dados pessoal do paciente. O sistema tem como sua principal função: Registrar as consultas, exames e laudos, realizadas pelo paciente com diversos médicos e especialistas ao longo de sua vida. Serão registrados no sistema dados tais como; nome do médico, especialidade, data da consulta, CRM, diagnóstico, solicitações e resultados de exames, laudos e pareceres.


### 1	COMPONENTES<br>
Integrantes do grupo:<br>
Eduardo Couto eduardocoouto@gmail.com<br>
Olavo Curatola olavo.curatola@gmail.com<br>
Lucas Garcia lucasoliveiragarcia@live.com<br>

### 2	INTRODUÇÃO E MOTIVAÇAO<br>
Este documento contém a especificação do projeto do banco de dados do HPAC<br>
A principal motivação para o desenvolvimento desse sistema é possibilitar uma maior segurança no uso de informações do paciente, no tocante a qualidade e confiabilidade da informação e tambem quanto a permissão de acesso a dados tão sensíveis. A idéia é construir ao longo da vida das pessoas um dossiê com todos os registros de seus problemas de saúde, com os resultados de exames e teste a cada momento de sua vida. Este dossiê deverá ser portado e gerenciado pelo paciente, podendo ser disponibilizado ou acessado por um médico sob sua autorização<br>
      
### 3	MINI-MUNDO<br>
O grupo deseja criar um sistema de informação para gerenciar as informações relacionadas às consultas médicas que as pessoas fazem  ao longo da vida, o intuito é que as mesmas tenham suas informações documentadas em nosso sistema e apresentem ao seu médico e evitem de
ter que falar todo o seu histórico a cada médico que for consultado.

O usuário deve fazer o login e digitar sua senha para entrar no sistema, caso já esteja cadastrado. Caso contrário, deverá fazer o cadastro, fornecendo nome completo, CPF, Identidade, endereço, telefone, e-mail, criando sua senha pessoal. Em seguida terá acesso as funcionalidade de criação, consulta e atualização de seu histórico. Podendo incluir exames, radiografias, tomografias, ressonâncias magnética, diagnósticos, laudos e comentários pertinentes. 
Além disso, o sistema deverá registrar todo o receituário prescrito para o paciente, bem como eventuais internações clinicas ou hospitalares, cirurgias e de mais procedimentos médicos.
O paciente poderá a qualquer momento atualizar seu histórico com a inserção de dados de novas consultas e exames, assim como poderá inserir resultados de exames antigos que eventualmente encontre em seus arquivos pessoais (em papel), podendo voltar na linha do tempo para completar informações e dar maior consistência ao seu dossiê.
O sistema deverá ser multiplataforma com acesso por smartphones e computadores pessoais, com acesso em tempo integral. Além disso, deverá possibilitar o acesso rápido aos dados.

### 4	RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
https://github.com/OlavoCuratola/BD2-HPAC/blob/master/Telas%20Smartphone.pdf<br>

4.1 TABELA DE DADOS DO SISTEMA:<br>
Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas. 
link para a tabela: https://github.com/OlavoCuratola/BD2-HPAC/blob/master/Tabela%20Dados%20Gerais%20Sistema%20-%20HPAC.xlsx


### 5	MODELO CONCEITUAL<br>
#### 5.1 NOTACAO ENTIDADE RELACIONAMENTO
https://github.com/OlavoCuratola/BD2-HPAC/blob/master/Conceitual%20HPAC3.pdf<br>
    
     5.2 NOTACAO UML (Caso esteja fazendo a disciplina de Projeto)

#### 5.3 DECISÕES DE PROJETO
    [atributo]: [descrição da decisão]
    
    EXEMPLO:
    a) Campo endereço: em nosso projeto optamos por um campo multivalorado e composto, pois a empresa 
    pode possuir para cada departamento mais de uma localização... 
    b) justifique!

#### 5.4 DESCRIÇÃO DOS DADOS 
    [objeto]: [descrição do objeto]
    
    EXEMPLO:
    CLIENTE: Tabela que armazena as informações relativas ao cliente<br>
    CPF: campo que armazena o número de Cadastro de Pessoa Física para cada cliente da empresa.<br>
    
    Tabela: receita	- receita do paciente
    Campo: ID_receita - ID
    Campo: data - data

    Tabela: medico	- médico
    Campo: ID_medico	- ID
    Campo: nome	- nome

    Tabela: laudo	- laudo do paciente
    Campo: ID_laudo	- ID
    Campo: data	- data

    Tabela: Exame	- exame do paciente
    Campo: IDExame	- ID
    Campo: Data	- Data

    Tabela: Consulta	- consulta do paciente
    Campo: Diagnostico	- Diagnóstico do médico sobre o paciente

    Tabela: paciente	- paciente
    Campo: ID_paciente	- ID
    Campo: identidade	- identidade
    Campo: cpf	- CPF
    Campo: nome	- nome
    Campo: CPF	- CPF
    Campo: data_nasc	- data
    Campo: endereço	- endereço
    Campo: telefone	- telefone
    Campo: login	- login de acesso ao sistema
    Campo: senha	- senha de acesso ao sistema

### 6	MODELO LÓGICO<br>
https://github.com/OlavoCuratola/BD2-HPAC/blob/master/Logico%20HPAC3.pdf<br>
### 7	MODELO FÍSICO<br>
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
#### 8.1 DETALHAMENTO DAS INFORMAÇÕES
        Detalhamento sobre as informações e processo de obtenção ou geração dos dados.
        Referenciar todas as fontes referentes a:
        a) obtenção dos dados
        b) obtenção de códigos reutilizados
        c) fontes de estudo para desenvolvimento do projeto
        
#### 8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELAS E INSERÇÃO DOS DADOS (ARQUIVO ÚNICO COM):
        a) inclusão das instruções para criação das tabelas e estruturas de amazenamento do BD
        b) inclusão das instruções de inserção dos dados nas referidas tabelas
        c) inclusão das instruções para execução de outros procedimentos necessários

### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
#### 9.1	GERACAO DE DADOS (MÍNIMO DE 10 REGISTROS PARA CADA TABELA NO BANCO DE DADOS)<br>

## Data de Entrega: (18/09/2017)

<br>
OBS: Incluir para os tópicos 9.2 e 9.3 as instruções SQL + imagens (print da tela) mostrando os resultados.<br>

#### 9.2	SELECT DAS TABELAS COM PRIMEIROS 10 REGISTROS INSERIDOS <br> 
    Data de Entrega: (Data a ser definida)
<br>

#### 9.3	SELECT DAS VISÕES COM PRIMEIROS 10 REGISTROS DA VIEW <br>
        a) Descrição da view sobre que grupos de usuários (operacional/estratégico) <br>
        e necessidade ela contempla.
        b) Descrição das permissões de acesso e usuários correlacionados (após definição <br>
        destas características)
    Data de Entrega: (Data a ser definida)
        c) as funcionalidades informadas no minimundo ou nos mockups(protótipos), que representarem 
        views do sistema (relatórios, informações disponíveis para os usuários, etc) devem estar 
        presentes aqui. 
<br>

#### 9.4	LISTA DE CODIGOS DAS FUNÇÕES, ASSERÇOES E TRIGGERS<br>
        Detalhamento sobre funcionalidade de cada código.
        a) Objetivo
        b) Código do objeto (função/trigger/asserção)
        c) exemplo de dados para aplicação
        d) resultados em forma de tabela/imagem
<br>

#### 9.5	Administração do banco de dados<br>
        Descrição detalhada sobre como serão executadas no banco de dados as <br>
        seguintes atividades.
        a) Segurança e autorização de acesso:
        b) Estimativas de aquisição de recursos para armazenamento e processamento da informação
        c) Planejamento de rotinas de manutenção e monitoramento do banco
        d) Plano com frequencia de análises visando otimização de performance
<br>

#### 9.6	GERACAO DE DADOS (MÍNIMO DE 1,5 MILHÃO DE REGISTROS PARA PRINCIPAL RELAÇAO)<br>
        a) principal tabela do sistema deve ter no mínimo 1,5 milhão de registros
        b) tabelas diretamente relacionadas a tabela principal 100 mil registros
        c) tabelas auxiliares de relacao multivalorada mínimo de 10 registros
        d) registrar o tempo de inserção em cada uma das tabelas do banco de dados
        e) especificar a quantidade de registros inseridos em cada tabela
        Para melhor compreensão verifiquem o exemplo na base de testes:<br>
        https://github.com/discipbd2/base-de-testes-locadora
        


#### 9.7	Backup do Banco de Dados<br>
        Detalhamento do backup.
        a) Tempo
        b) Tamanho
        c) Teste de restauração (backup)
        d) Tempo para restauração
        e) Teste de restauração (script sql)
        f) Tempo para restauração (script sql)
<br>

Data de Entrega: (Data a ser definida)
<br>

#### 9.8	APLICAÇAO DE ÍNDICES E TESTES DE PERFORMANCE<br>
    a) Lista de índices, tipos de índices com explicação de porque foram implementados nas consultas 
    b) Performance esperada VS Resultados obtidos
    c) Tabela de resultados comparando velocidades antes e depois da aplicação dos índices (constando velocidade esperada com planejamento, sem indice e com índice Vs velocidade de execucao real com índice e sem índice).
    d) Escolher as consultas mais complexas para serem analisadas (consultas com menos de 2 joins não serão aceitas)
    e) As imagens do Explain devem ser inclusas no trabalho, bem como explicações sobre os resultados obtidos.
    f) Inclusão de tabela mostrando as 10 execuções, excluindo-se o maior e menor tempos para cada consulta e 
    obtendo-se a media dos outros valores como resultado médio final.
<br>
    Data de Entrega: (Data a ser definida)
<br>   

#### 9.9	ANÁLISE DOS DADOS COM ORANGE<br>    
        a) captura das informaçõs
        b) integração com banco de dados em desenvolvimento
        c) aplicação de algoritmos e interpretação dos resultados
        c) atualização da documentação do trabalho incluindo a mineração de dados
<br>
    Data de Entrega: (Data a ser definida)
<br>

### 10	ATUALIZAÇÃO DA DOCUMENTAÇÃO/ SLIDES E ENTREGA FINAL<br>
<br>
    Data de Entrega: (Data a ser definida)
<br>

### 11	DIFICULDADES ENCONTRADAS PELO GRUPO<br>  

       
### 12  FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>
    
##### About Formatting
    https://help.github.com/articles/about-writing-and-formatting-on-github/
    
##### Basic Formatting in Git
    
    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests
    
    
##### Working with advanced formatting
    https://help.github.com/articles/working-with-advanced-formatting/
#### Mastering Markdown
    https://guides.github.com/features/mastering-markdown/

### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.
1. Caso existam arquivos com conteúdos sigilosos, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário deste GIT, para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.


Link para BrModelo:<br>
http://sis4.com/brModelo/brModelo/download.html
<br>


Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")



