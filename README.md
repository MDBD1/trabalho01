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
    a) Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas/registros de dados.
    b) Esta tabela tem a intenção de simular um relatório com todos os dados que serão armazenados
    e deve ser criada antes do modelo conceitual
    c) Após criada esta tabela não deve ser modificada, pois será comparada com os resultados finais na conclusão do trabalho
    
![Tabela da Empresa Neworld](https://github.com/MDBD1/trabalho01/blob/master/arquivos/TabelaEmpresaNeworld2.xlsx)
    
>## Marco de Entrega 01 em: (24/03/2018)<br>
### 5.MODELO CONCEITUAL<br>
   
        
![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/2018-07-03%20(1).png)
    
    
    
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

* Campo Empresa do ônibus: optamos por esse campo para que o usuário saiba qual empresa atua em cada ponto de ônibos.

* Campo Rua/Avenida/Alameda, Bairro, Cidade, Estado: colocamos esse campo para que o ponto de ônibus seja 
melhor indentificado pelo sistema.
* Não não fizemos o tópico 9.4 letra b, pois o nosso trabalho não precisa da informação data.
    
#### 5.3 DESCRIÇÃO DOS DADOS
    [objeto]: [descrição do objeto]
    
USUÁRIO: Tabela que armazenas as informações relativas ao usuário<br>
E-MAIL: campo que armazena o e-mail de cada usuário cadastrado no sistema<br>
SENHA: campo que armazena a senha de cada usuário<br>
NOME: campo que armazena o nome de cada usuário<br>
RUA_AVENIDA_ALAMEDA, BAIRRO, CIDADE, ESTADO e NÚMERO_DA_CASA: campos que armazenam o endereço do usuário, sua rua,
bairro, cidade, estado e número de sua casa, respectivamente.<br>

ÔNIBUS: Tabela que armazena as informações relativas aos ônibus<br>
NÚMERO_DO_ÔNIBUS: campo que armazena o número que identifica o ônibus<br>
NÚMERO_DA_LINHA:  campo que armazena a linha do ônibus<br>
HORÁRIO_DE_SAÍDA: campo que armazena os horários que os respectivos ônibus saem de seu ponto inicial<br>
HORÁRIO_DE_CHAGADO: campo que armazena os hosrários de chegada que os ônibus chegam em seu ponto final<br>
ITINERÁRIO:  campo que armazena os locais em que os ônibus circulam<br>

PONTO_DE_ÔNIBUS: Tabela que armazena as informções relativas aos pontos de ônibus<br>
NÚMERO_DO_PONTO: campo que armazena o número que indentifica o  ponto de ôonibus.
EMPRESA_DO_ÔNIBUS: campo que armazena a empresa dos ônibus que opera no ponto de ônibus<br>
RUA_AVENIDA_ALAMEDA, BAIRRO, CIDADE e ESTADO: campos que armazenam o endereço do ponto de ônibus, sua rua,<br>
bairro, cidade e estado respectivamente.<br>  

ÔNIBUS_PONTO: tabela que armazena as informações que relacionam o ÔNIBUS com seus PONTOS DE ÔNIBUS<BR>
    
>## Marco de Entrega 01 em: (12/05/2018)<br>
### 6 MODELO LÓGICO<br>
   ![Modelo lógico](https://github.com/MDBD1/trabalho01/blob/master/imagens/2018-07-03.png)
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
        a) inclusão das instruções de inserção dos dados nas tabelas criadas pelo script de modelo físico
        b) formato .SQL
        
insert into USUARIO(email,senha,nome,rua_avenida, bairro, cidade, estado, n_da_casa)
values ('fernadasilva@email.com','tuyghj678','Fernanda da Silva', 'Avenida Fernando Ferrari','Goiabeiras','Vitória','Espírito Santo','56'),('mariaclara@email.com','sckopdnefj8','Maria Clara dos Santos','Emanuel Ribeiro','Laranjeiras','Serra','Espírito Santo' 
,'1600'),('robertaOliveira@email.com','qreytjukfd','Roberta Oliveira','Garrafa Furada','Churrasco','Vila Velha','Espírito Santo','1601'),
('dsgfdhsj@email.com','bibibibibi','Mark Pereira','Batata','Carne Moida','Viana','Espírito Santo' ,'1602'),
('blablabla@email.com','qwer1234','Beatris dos Santos','Reta da penha','Patinho','São Paulo','São Paulo','1603'),
('lkdaqwe@email.com','123890iop','Jackson Wang','Melancia','Lombo','Cariacica','Espírito Santo','1604'),
('weakSempre@email.com','universo123','Karen Bachini','Abóbora','Bife','Serra','Espírito Santo','1605'),
('bliblipimpim@gmail','kkj1234','Maria Carolina Da Silva','Abacate','Picanha','Serra','Espírito Santo','1606'),
('guiSilveira@email.com','6543212','Guilherme Silveira','Gato Preto','Tigre',' Vitória da Conquista','Bahia','1607'),
('jubilix@gmail.com','coisalinda','Juliana Vasconcelos','Rua Anchieta','Valparaíso','Serra','Espírito Santo', '50');

insert into onibus(n_onibus,n_linha,saida,chegada,itinerario)
values (234567, 400,'12:00:00','12:30:00','Avenida Paulo Pereira Gomes'),(534285, 289,'13:10:00','13:50:00','Rua Anchieta'),
(123454, 567,'11:00:00','11:50:00','Avenida Fernando Ferrari'),(876557, 900,'05:40:00','06:00:00','Avenida Norte Sul'),
(645323, 432,'08:40:00','09:40:00','Avenida Central'),(785444, 72,'09:50:00','16:30:00','Avenida Eudes Scherrer de Souza'),
(45689,	789,'10:10:00','11:40:00','Civit ll'),(978678,500,'11:55:00','12:55:00','Avenida João Palácio'),
(12345,	121,'12:40:00','13:45:00','Avenida Américo Buiaz'),(64321, 560,'11:52:00','14:15:00','Avenida Guarapari');

insert into ponto_de_onibus(n_ponto,tipo_de_onibus,rua_avenida,bairro,cidade,estado)
values (128937,'Transcol','Reta da Penha','Santa Helena','Vitória','Espírito Santo'),
(12345,'Transcol','Avenida Fernando Ferrari','Jardim da Penha','Vitória','Espírito Santo'),
(87654,'Transcol','Avenida Eudes Scherrer de Souza','Laranjeiras','Serra','Espírito Santo'),
(57687,'Seletivo','Rua Anchieta','Santa Luzia','Serra','Espírito Santo'),
(53034,'Seletivo','Avenida Norte Sul','Rosário de Fátima','Serra','Espírito Santo'),
(96543,'Transcol','Avenida Saturnino de Brito','Santa Helena','Vitória','Espírito Santo'),
(1006,'Transcol','Rodovia Governado Mário Covas','Rosário de Fátima','Serra','Espírito Santo'),
(12456,'Transcol','Rua Antônio Ataíde','Itapuã','Vila Velha','Espírito Santo'),
(123090,'Transcol','Avenida Luciano das Neves','Itapuã','Vila Velha','Espírito Santo'),
(4893095,'Seletivo','Avenida Guarapari','Santa Luzia','Serra','Espírito Santo');

insert into ponto_onibus(FK_ONIBUS_n_onibus,FK_PONTO_DE_ONIBUS_n_ponto) values (234567,128937),(534285,12345),(123454,87654),(876557,57687),(645323,53034),
(785444,96543),(45689,1006),(978678,12456),(12345,123090),(64321,4893095);

insert into acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS( FK_USUARIO_email,FK_PONTO_DE_ONIBUS_n_ponto,FK_ONIBUS_n_onibus)
values ('fernadasilva@email.com',128937,234567),
('mariaclara@email.com',12345,534285),
('robertaOliveira@email.com',87654,123454),
('dsgfdhsj@email.com',57687,876557),
('blablabla@email.com',53034,645323),
('lkdaqwe@email.com',96543,785444),
('weakSempre@email.com',1006,45689),
('bliblipimpim@gmail',12456,978678),
('guiSilveira@email.com',123090,12345),
('jubilix@gmail.com',4893095,64321);

<br>
#### 8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script
        (create para tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL
        
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
    
insert into USUARIO(email,senha,nome,rua_avenida, bairro, cidade, estado, n_da_casa)
values ('fernadasilva@email.com','tuyghj678','Fernanda da Silva', 'Avenida Fernando Ferrari','Goiabeiras','Vitória','Espírito Santo','56'),('mariaclara@email.com','sckopdnefj8','Maria Clara dos Santos','Emanuel Ribeiro','Laranjeiras','Serra','Espírito Santo' 
,'1600'),('robertaOliveira@email.com','qreytjukfd','Roberta Oliveira','Garrafa Furada','Churrasco','Vila Velha','Espírito Santo','1601'),
('dsgfdhsj@email.com','bibibibibi','Mark Pereira','Batata','Carne Moida','Viana','Espírito Santo' ,'1602'),
('blablabla@email.com','qwer1234','Beatris dos Santos','Reta da penha','Patinho','São Paulo','São Paulo','1603'),
('lkdaqwe@email.com','123890iop','Jackson Wang','Melancia','Lombo','Cariacica','Espírito Santo','1604'),
('weakSempre@email.com','universo123','Karen Bachini','Abóbora','Bife','Serra','Espírito Santo','1605'),
('bliblipimpim@gmail','kkj1234','Maria Carolina Da Silva','Abacate','Picanha','Serra','Espírito Santo','1606'),
('guiSilveira@email.com','6543212','Guilherme Silveira','Gato Preto','Tigre',' Vitória da Conquista','Bahia','1607'),
('jubilix@gmail.com','coisalinda','Juliana Vasconcelos','Rua Anchieta','Valparaíso','Serra','Espírito Santo', '50');

insert into onibus(n_onibus,n_linha,saida,chegada,itinerario)
values (234567, 400,'12:00:00','12:30:00','Avenida Paulo Pereira Gomes'),(534285, 289,'13:10:00','13:50:00','Rua Anchieta'),
(123454, 567,'11:00:00','11:50:00','Avenida Fernando Ferrari'),(876557, 900,'05:40:00','06:00:00','Avenida Norte Sul'),
(645323, 432,'08:40:00','09:40:00','Avenida Central'),(785444, 72,'09:50:00','16:30:00','Avenida Eudes Scherrer de Souza'),
(45689,	789,'10:10:00','11:40:00','Civit ll'),(978678,500,'11:55:00','12:55:00','Avenida João Palácio'),
(12345,	121,'12:40:00','13:45:00','Avenida Américo Buiaz'),(64321, 560,'11:52:00','14:15:00','Avenida Guarapari');

insert into ponto_de_onibus(n_ponto,tipo_de_onibus,rua_avenida,bairro,cidade,estado)
values (128937,'Transcol','Reta da Penha','Santa Helena','Vitória','Espírito Santo'),
(12345,'Transcol','Avenida Fernando Ferrari','Jardim da Penha','Vitória','Espírito Santo'),
(87654,'Transcol','Avenida Eudes Scherrer de Souza','Laranjeiras','Serra','Espírito Santo'),
(57687,'Seletivo','Rua Anchieta','Santa Luzia','Serra','Espírito Santo'),
(53034,'Seletivo','Avenida Norte Sul','Rosário de Fátima','Serra','Espírito Santo'),
(96543,'Transcol','Avenida Saturnino de Brito','Santa Helena','Vitória','Espírito Santo'),
(1006,'Transcol','Rodovia Governado Mário Covas','Rosário de Fátima','Serra','Espírito Santo'),
(12456,'Transcol','Rua Antônio Ataíde','Itapuã','Vila Velha','Espírito Santo'),
(123090,'Transcol','Avenida Luciano das Neves','Itapuã','Vila Velha','Espírito Santo'),
(4893095,'Seletivo','Avenida Guarapari','Santa Luzia','Serra','Espírito Santo');

insert into ponto_onibus(FK_ONIBUS_n_onibus,FK_PONTO_DE_ONIBUS_n_ponto) values (234567,128937),(534285,12345),(123454,87654),(876557,57687),(645323,53034),
(785444,96543),(45689,1006),(978678,12456),(12345,123090),(64321,4893095);

insert into acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS( FK_USUARIO_email,FK_PONTO_DE_ONIBUS_n_ponto,FK_ONIBUS_n_onibus)
values ('fernadasilva@email.com',128937,234567),
('mariaclara@email.com',12345,534285),
('robertaOliveira@email.com',87654,123454),
('dsgfdhsj@email.com',57687,876557),
('blablabla@email.com',53034,645323),
('lkdaqwe@email.com',96543,785444),
('weakSempre@email.com',1006,45689),
('bliblipimpim@gmail',12456,978678),
('guiSilveira@email.com',123090,12345),
('jubilix@gmail.com',4893095,64321);

<br>
        
#### 8.3 INCLUSÃO DO SCRIPT PARA EXCLUSÃO DE TABELAS EXISTENTES, CRIAÇÃO DE TABELA NOVAS E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script
        (Drop table + Create de tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL
  
        
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
    
insert into USUARIO(email,senha,nome,rua_avenida, bairro, cidade, estado, n_da_casa)
values ('fernadasilva@email.com','tuyghj678','Fernanda da Silva', 'Avenida Fernando Ferrari','Goiabeiras','Vitória','Espírito Santo','56'),('mariaclara@email.com','sckopdnefj8','Maria Clara dos Santos','Emanuel Ribeiro','Laranjeiras','Serra','Espírito Santo' 
,'1600'),('robertaOliveira@email.com','qreytjukfd','Roberta Oliveira','Garrafa Furada','Churrasco','Vila Velha','Espírito Santo','1601'),
('dsgfdhsj@email.com','bibibibibi','Mark Pereira','Batata','Carne Moida','Viana','Espírito Santo' ,'1602'),
('blablabla@email.com','qwer1234','Beatris dos Santos','Reta da penha','Patinho','São Paulo','São Paulo','1603'),
('lkdaqwe@email.com','123890iop','Jackson Wang','Melancia','Lombo','Cariacica','Espírito Santo','1604'),
('weakSempre@email.com','universo123','Karen Bachini','Abóbora','Bife','Serra','Espírito Santo','1605'),
('bliblipimpim@gmail','kkj1234','Maria Carolina Da Silva','Abacate','Picanha','Serra','Espírito Santo','1606'),
('guiSilveira@email.com','6543212','Guilherme Silveira','Gato Preto','Tigre',' Vitória da Conquista','Bahia','1607'),
('jubilix@gmail.com','coisalinda','Juliana Vasconcelos','Rua Anchieta','Valparaíso','Serra','Espírito Santo', '50');

insert into onibus(n_onibus,n_linha,saida,chegada,itinerario)
values (234567, 400,'12:00:00','12:30:00','Avenida Paulo Pereira Gomes'),(534285, 289,'13:10:00','13:50:00','Rua Anchieta'),
(123454, 567,'11:00:00','11:50:00','Avenida Fernando Ferrari'),(876557, 900,'05:40:00','06:00:00','Avenida Norte Sul'),
(645323, 432,'08:40:00','09:40:00','Avenida Central'),(785444, 72,'09:50:00','16:30:00','Avenida Eudes Scherrer de Souza'),
(45689,	789,'10:10:00','11:40:00','Civit ll'),(978678,500,'11:55:00','12:55:00','Avenida João Palácio'),
(12345,	121,'12:40:00','13:45:00','Avenida Américo Buiaz'),(64321, 560,'11:52:00','14:15:00','Avenida Guarapari');

insert into ponto_de_onibus(n_ponto,tipo_de_onibus,rua_avenida,bairro,cidade,estado)
values (128937,'Transcol','Reta da Penha','Santa Helena','Vitória','Espírito Santo'),
(12345,'Transcol','Avenida Fernando Ferrari','Jardim da Penha','Vitória','Espírito Santo'),
(87654,'Transcol','Avenida Eudes Scherrer de Souza','Laranjeiras','Serra','Espírito Santo'),
(57687,'Seletivo','Rua Anchieta','Santa Luzia','Serra','Espírito Santo'),
(53034,'Seletivo','Avenida Norte Sul','Rosário de Fátima','Serra','Espírito Santo'),
(96543,'Transcol','Avenida Saturnino de Brito','Santa Helena','Vitória','Espírito Santo'),
(1006,'Transcol','Rodovia Governado Mário Covas','Rosário de Fátima','Serra','Espírito Santo'),
(12456,'Transcol','Rua Antônio Ataíde','Itapuã','Vila Velha','Espírito Santo'),
(123090,'Transcol','Avenida Luciano das Neves','Itapuã','Vila Velha','Espírito Santo'),
(4893095,'Seletivo','Avenida Guarapari','Santa Luzia','Serra','Espírito Santo');

insert into ponto_onibus(FK_ONIBUS_n_onibus,FK_PONTO_DE_ONIBUS_n_ponto) values (234567,128937),(534285,12345),(123454,87654),(876557,57687),(645323,53034),
(785444,96543),(45689,1006),(978678,12456),(12345,123090),(64321,4893095);

insert into acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS( FK_USUARIO_email,FK_PONTO_DE_ONIBUS_n_ponto,FK_ONIBUS_n_onibus)
values ('fernadasilva@email.com',128937,234567),
('mariaclara@email.com',12345,534285),
('robertaOliveira@email.com',87654,123454),
('dsgfdhsj@email.com',57687,876557),
('blablabla@email.com',53034,645323),
('lkdaqwe@email.com',96543,785444),
('weakSempre@email.com',1006,45689),
('bliblipimpim@gmail',12456,978678),
('guiSilveira@email.com',123090,12345),
('jubilix@gmail.com',4893095,64321);

drop table acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS;
drop table ponto_onibus;
drop table USUARIO;
drop table ONIBUS;
drop table PONTO_DE_ONIBUS;


  
  
  
### 9 TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1 CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>

select * from usuario;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/newusuario.png)<br>

select * from onibus;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/newonibus.png)<br>

select * from ponto_de_onibus;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/newponto_de_onibus.png)<br>

select * from ponto_onibus;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/newponto_onibus.png)<br>

select * from acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/newisso.png)<br>
<br>

#### 9.2 CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>

select * from usuario where cidade='Serra';<br>
select nome from usuario where n_da_casa='1601';<br>
select * from usuario where bairro<>'Valparaíso';<br>
select * from onibus where n_onibus=234567;<br>
<br>

#### 9.3 CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)<br>
  
    
a)<br>

select estado from usuario where estado='Espírito Santo' and n_da_casa='50';<br>
select cidade from usuario where estado='Espírito Santo' or estado='Bahia';<br>
select n_onibus from onibus where saida='12:00:00' and chegada='12:30:00';<br>
select * from ponto_de_onibus where n_ponto is not null;<br>
select * from onibus where n_onibus>500000 and n_linha>400 or n_onibus<200000 and n_linha<200;<br>

<br>

b)<br>

select n_linha+1000 from onibus where n_onibus<60000;<br>
select n_onibus%2 from onibus where n_onibus>200000;<br>
select n_linha*1.1 from ponto_de_onibus;<br>
<br>
c)

SELECT * FROM usuario as user WHERE nome LIKE 'J%';<br>
SELECT * FROM onibus as bus WHERE bus.n_linha LIKE 'J%' and bus.itinerario='Rua Anchieta';<br>
SELECT * FROM ponto_de_onibus as pnt WHERE nome LIKE 'J%';<br>

<br>
#### 9.4 CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.

a)<br>

select * from usuario where nome like'J%';<br>
select * from onibus where itinerario like'A%';<br>
select * from ponto_de_onibus where estado like'S%';<br>
select * from ponto_de_onibus where estado like'%Paulo';<br>
select * from usuario where bairro like'L%';<br>

<br>

b)<br>

Nós não fizemos esse tópico, pois o nosso trabalho não precisa da informação data.

<br>

#### 9.5 ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>

update usuario set nome='Júlia Ferreira' where senha='coisalinda';<br>
update onibus set n_onibus=908978 where itinerario='Avenida Guarapari';<br>
update ponto_de_onibus set tipo_de_onibus='Seletivo' where n_ponto=12345;<br>

delete from usuario where n_da_casa='56';<br>
delete from onibus where n_onibus=234567;<br>
delete from ponto_de_onibus where bairro='Rosário de Fátima';<br>
<br>
#### 9.6 CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br>
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
        
a)<br>
select nome,n_onibus,n_ponto from usuario,onibus,ponto_de_onibus order by n_ponto;
<br>
        
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


        
        


    





