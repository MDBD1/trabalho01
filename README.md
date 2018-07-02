# TRABALHO 01:  Título do Trabalho
Trabalho desenvolvido durante a disciplina de Banco de Dados do Integrado
# Sumário
### 1. COMPONENTES<br>
Integrantes do grupo<br>
Mariana Polli Gusmão: mancadinha121@gmail.com<br>
Kezia de Jesus de Souza: keziajsouz@gmail.com<br>
Júlia Ferreira da Silva: juliafds2001@gmail.com<br>

### 2.INTRODUÇÃO E MOTIVAÇAO<br>
Este documento contém a especificação do projeto do banco de dados TimeBus
<br>e motivação da escolha realizada. <br>
>A empresa “Neworld” tem como objetivo desenvolver as cidades, proporcionando maior qualidade de vida e organização, usando a tecnologia para melhorar a rotina da população, apresentando projetos que atuaram em várias áreas dentro da sociedade. A empresa está crindo um novo projeto de um aplicativo, chamado de TimeBus, que proporcionará uma melhora a mobilidade urbana, deixando as pessoas informadas sobre os transportes públicos, possibilitando que as pessoas se programem e se organizem da melhor forma para evitar, por exemplo, superlotação nos pontos de ônibus. Para isso, a empresa aperfeiçoará os pontos de ônibus públicos (para que a pessoa tenha acesso ao aplicativo dentro do ponto, com aparelhos digitais de entrada,"touch", e saída, tela), permitindo que a população possa ter acesso às informações dos ônibus, como o local em que o mesmo se encontra, horário de chegada, e engarrafamentos nas proximidades, pelos aparelho móveis e pelos aparelhos dos pontos de ônibus.

 
### 3.MINI-MUNDO Novo<br>

> O “TimeBus”, sistema proposto para a "Neworld” conterá as informações aqui detalhadas. O sistema terá como entrada o local onde o usuário acessa as informações sobre o ônibus e os pontos de ônibus. Ele utilizará o nome, e-mail, senha, e o endereço (rua, avenida, bairro, cidade, etc) dos usuários para fazer o cadastro no sistema. O sistema também irá pedir as informações sobre os pontos de ônibus: número do ponto, empresas de ônibus que passam pelo ponto referido (tipo do ônibus), e o endereço do ponto. Depois será feita a leitura das informações dos ônibus em questão: número do ônibus, número da linha, horário (chegada e saída) e o itinerário.  E irá contar com o waze para identificar os pontos de engarrafamento (trânsito pesado). Desse modo, teremos o projeto “TimeBus” desenvolvido.

### 4.RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>

![Alt text](https://github.com/discipbd1/trab01/blob/master/balsamiq.png?raw=true "Title")
![Arquivo PDF do Protótipo Balsamiq feito para Neworld](https://github.com/MDBD1/trabalho01/blob/master/arquivos/MDBD%20F%20TimeBus.pdf)

#### 4.1 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
    
    
> A Empresa Neworld precisa inicialmente dos seguintes relatórios:
* Relatório que informe quais são os usuários presentes no sistema incluindo as seguintes informações:
email do usuário, senha do usuário, nome e seu endereço(Rua, bairro, cidade, estado, número da casa).
* Relatório dos ônibus presentes no sistema incluindo as seguintes informações: número do ônibus,
número de linha do ônibus, horários de saída e chegada do ônibus e seu itinerário.
* Relatório dos pontos de ônibus do sistema incluindo as seguintes informações: número do ponto, 
empresa do ônibus(que passa por aquele ponto) e sua localização(rua, bairro, cidade, estado).
* Relatório de ônibus com ponto de ônibus incluindo as seguintes informações: número do ônibus e 
número do ponto de ônibus.

 
#### 4.2 TABELA DE DADOS DO SISTEMA:
   
    
![ Tabela de dados da Empresa Neworld](https://github.com/MDBD1/trabalho01/blob/master/arquivos/TabelaEmpresaNeworld2.xlsx "Tabela - Empresa Neworld")
    
>## Marco de Entrega 01 em: (24/03/2018)<br>
### 5.MODELO CONCEITUAL<br>
   
        
![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/2018-06-30%20(5).png)
    
    
    
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: [Nomes dos que participaram na avaliação]
    [Grupo02]: [Nomes dos que participaram na avaliação]
## Marco de Entrega 01 em: (20/04/2018)<br>
#### 5.2 DECISÕES DE PROJETO
    [atributo]: [descrição da decisão]
   
* Campo E-mail: em nosso projeto optamos por essa campo, pois caso precisemos informa algo ao usuário
teremos o seu contato.

* Campo Senha: colocomos essa campo para que o usuário tenha privacidade e segurança sobre seu login.

* Campo Nome: optamos por esse campo para ter informações a mais sobre o cliente.

* Campo Rua/Avenida/Alameda, Bairro, Cidade, Estado, Número da casa: optamos por esses campos para que 
sua localizaçõa seje clara e facilite ao sistema encontrar pontos de ônibus mais próximos ao usuário.

* Campo Número do ônibus: esse campo foi colocado para que possamos melhor indentificar o ônibus.

* Campo Número da linha: optamos por esse campo pois iremos relacioná-lo com o itinerário, e também
para o usuário indentificar o ônibus.

* Compo Horário de saída e chegada: Optamos por esse campo para facilitar ao sistema de mostrar ao usuário
o tempo que falta pra tal ônibus chegar a tal ponto de ônibus.

* Campo Itinerário: colocamos esse campo para que o usuário tenah acesso ao caminho que tal ônibus pecorre,  
para melhor indentificar o horário do ônibus, e para dizer quais pontos esse ônibus passa.

* Campo Número do ponto: serve para melhor indentificarmos cada ponto de ônibus, e ralacioná-lo com os números dos ônibus
que ali passam.

* Campo Empresa doo ônibus: optamos por esse campo para que o usuário saiba qual empresa atua em cada ponto de ônibos.

* Campo Rua/Avenida/Alameda, Bairro, Cidade, Estado: colocamos esse campo para que o ponto de ônibus seja 
melhor indentificado pelo sistema.

    
#### 5.3 DESCRIÇÃO DOS DADOS
    [objeto]: [descrição do objeto]
    
USUÁRIO: Tabela que armazenas as informações relativas ao usuário<br>
E-MAIL: campo que armazena o e-mail de cada usuário cadastrado no sistema<br>
SENHA: campo que armazena a senha de cada usuário<br>
NOME: campo que armazena o nome de cada usuário<br>
RUA/AVENIDA/ALAMEDA, BAIRRO, CIDADE, ESTADO e NÚMERO DA CASA: campos que armazenam o endereço do usuário, sua rua,
bairro, cidade, estado e número de sua casa, respectivamente.<br>

ÔNIBUS: Tabela que armazena as informações relativas aos ônibus<br>
NÚMERO DO ÔNIBUS: campo que armazena o número que identifica o ônibus<br>
NÚMERO DA LINHA:  campo que armazena a linha do ônibus<br>
HORÁRIO DE SAÍDA: campo que armazena os horários que os respectivos ônibus saem de seu ponto inicial<br>
HORÁRIO DE CHAGADO: campo que armazena os hosrários de chegada que os ônibus chegam em seu ponto final<br>
ITINERÁRIO:  campo que armazena os locais em que os ônibus circulam<br>

PONTO DE ÔNIBUS: Tabela que armazena as informções relativas aos pontos de ônibus<br>
NÚMERO DO PONTO: campo que armazena o número que indentifica o  ponto de ôonibus.
EMPRESA DO ÔNIBUS: campo que armazena a empresa dos ônibus que opera no ponto de ônibus<br>
RUA/AVENIDA/ALAMEDA, BAIRRO, CIDADE e ESTADO: campos que armazenam o endereço do ponto de ônibus, sua rua,<br>
bairro, cidade e estado respectivamente.<br>  

ÔNIBUS PONTO: tabela que armazena as informações que relacionam o ÔNIBUS com seus PONTOS DE ÔNIBUS<BR>
    
>## Marco de Entrega 01 em: (12/05/2018)<br>
### 6 MODELO LÓGICO<br>
   ![Modelo lógico](https://github.com/MDBD1/trabalho01/blob/master/imagens/2018-07-02.png)
### 7 MODELO FÍSICO<br>
       

CREATE TABLE USUARIO (
    email varchar(80) PRIMARY KEY,
    senha varchar(80),
    nome varchar(80),
    n_da_casa varchar(80),
    rua_avenida  varchar(255),
    bairro varchar(100),
    estado varchar(100),
    cidade varchar(100)
);

CREATE TABLE ONIBUS (
    n_onibus int PRIMARY KEY,
    n_linha int,
    saida time,
    chegada time,
    itinerario varchar(255)
);

CREATE TABLE PONTO_DE_ONIBUS (
    n_ponto int PRIMARY KEY,
    tipo_de_onibus varchar(80),
    cidade varchar(100),
    rua_avenida varchar(255),
    bairro varchar(100),
    estado varchar(100)
);

CREATE TABLE ENTRADA (
);

CREATE TABLE acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS (
    FK_USUARIO_email varchar(80),
    FK_PONTO_DE_ONIBUS_n_ponto int,
    FK_ONIBUS_n_onibus int
);

CREATE TABLE ponto_onibus (
    FK_ONIBUS_n_onibus int,
    FK_PONTO_DE_ONIBUS_n_ponto int
);
 
ALTER TABLE acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS ADD CONSTRAINT FK_acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS_0
    FOREIGN KEY (FK_USUARIO_email)
    REFERENCES USUARIO (email)
    ON DELETE NO ACTION ON UPDATE NO ACTION;
 
ALTER TABLE acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS ADD CONSTRAINT FK_acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS_1
    FOREIGN KEY (FK_PONTO_DE_ONIBUS_n_ponto)
    REFERENCES PONTO_DE_ONIBUS (n_ponto)
    ON DELETE NO ACTION ON UPDATE NO ACTION;
 
ALTER TABLE acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS ADD CONSTRAINT FK_acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS_2
    FOREIGN KEY (FK_ONIBUS_n_onibus)
    REFERENCES ONIBUS (n_onibus)
    ON DELETE NO ACTION ON UPDATE NO ACTION;
 
ALTER TABLE ponto_onibus ADD CONSTRAINT FK_ponto_onibus_0
    FOREIGN KEY (FK_ONIBUS_n_onibus)
    REFERENCES ONIBUS (n_onibus)
    ON DELETE SET NULL ON UPDATE CASCADE;
 
ALTER TABLE ponto_onibus ADD CONSTRAINT FK_ponto_onibus_1
    FOREIGN KEY (FK_PONTO_DE_ONIBUS_n_ponto)
    REFERENCES PONTO_DE_ONIBUS (n_ponto)
    ON DELETE SET NULL ON UPDATE CASCADE;      
        
### 8 INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
#### 8.1 DETALHAMENTO DAS INFORMAÇÕES
        a) inclusão das instruções de inserção dos dados nas tabelas criadas pelo script de modelo físic
        b) formato .SQL
#### 8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script
        (create para tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL
#### 8.3 INCLUSÃO DO SCRIPT PARA EXCLUSÃO DE TABELAS EXISTENTES, CRIAÇÃO DE TABELA NOVAS E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script
        (Drop table + Create de tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL

### 9 TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1 CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>
#### 9.2 CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>
#### 9.3 CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas
#### 9.4 CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.

    
#### 9.5 ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>

#### 9.6 CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br>
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
        
## Marco de Entrega 02 em: (16/06/2018)<br>
### ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO SEMESTRAL (Mínimo 6 e Máximo 10)<br>
<br>
#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>

#### 9.8	CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4)<br>
#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho
#### 9.10	SUBCONSULTAS (Mínimo 3)<br>

#### 9.11	LISTA DE CODIGOS DAS FUNÇÕES E TRIGGERS<br>
        Detalhamento sobre funcionalidade de cada código.
        a) Objetivo
        b) Código do objeto (função/trigger)
        c) exemplo de dados para aplicação
        d) resultados em forma de tabela/imagem
<br>

#### 9.12 GERACAO DE DADOS (MÍNIMO DE 100 MIL REGISTROS PARA PRINCIPAL RELAÇAO)<br>
        a) principal tabela do sistema deve ter no mínimo 100 mil registros
        b) tabelas diretamente relacionadas a tabela principal 10 mil registros
        c) tabelas auxiliares de relacao multivalorada mínimo de 10 registros
        d) registrar o tempo de inserção em cada uma das tabelas do banco de dados
        e) especificar a quantidade de registros inseridos em cada tabela
        Para melhor compreensão verifiquem o exemplo na base de testes:<br>
        https://github.com/discipbd2/base-de-testes-locadora
        
#### 9.13 Backup do Banco de Dados<br>
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

#### 9.14	APLICAÇAO DE ÍNDICES E TESTES DE PERFORMANCE<br>
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

### 10	ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO FINAL (Mínimo 6 e Máximo 10)<br>
<br>
    Data de Entrega: (Data a ser definida)
<br>

### 11 Backup completo do banco de dados postgres 
    a) deve ser realizado no formato "backup" 
        (Em Dump Options #1 Habilitar opções Don't Save Owner e Privilege)
    b) antes de postar o arquivo no git o mesmo deve ser testado/restaurado por outro grupo de alunos/dupla
    c) informar aqui o grupo de alunos/dupla que realizou o teste.
    
### 12 TUTORIAL COMPLETO DE PASSOS PARA RESTAURACAO DO BANCO E EXECUCAO DE PROCEDIMENTOS ENVOLVIDOS NO TRABALHO PARA OBTENÇÃO DOS RESULTADOS<br>
        a) Outros grupos deverão ser capazes de restaurar o banco
        b) executar todas as consultas presentes no trabalho
        c) executar códigos que tenham sido construídos para o trabalho
        d) realizar qualquer procedimento executado pelo grupo que desenvolveu o trabalho
### 13 DIFICULDADES ENCONTRADAS PELO GRUPO<br> 
    
>## Marco de Entrega 04/Entrega Final em: (Data definida no cronograma)<br>
       
### 14  FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/
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


        
        


    





