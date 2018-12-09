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
   
        
![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/ultimobrmodelo.png)
    
    
#### 5.1 Validação do Modelo Conceitual
    [Biblioteca Virtual]: [Marina Milagres, Gustavo Duntra]
    [Semafro Up]: [Christian, Gabriel]
## Marco de Entrega 01 em: (20/04/2018)<br>
#### 5.2 DECISÕES DE PROJETO
    [atributo]: [descrição da decisão]
   Usuário:
   
Campo E-mail (email): em nosso projeto optamos por essa campo, pois caso precisemos informa algo ao usuário teremos o seu contato.

Campo Senha (senha): colocomos essa campo para que o usuário tenha privacidade e segurança sobre seu login.

Campo Nome (nome): optamos por esse campo para ter informações a mais sobre o cliente.

Campo Número da Casa (n_da_casa): optamos por esse campo para melhor compreender o endereço do usuário.

Campo Código (codigo): criamos esse campo para que a consulta sobre cada usuário fique mais acessível, assim cada usuário tem sua própria “identidade”.

   Ônibus: 
 
Campo Número do ônibus (n_onibus): esse campo foi colocado para que possamos melhor indentificar o ônibus.

Campo Número da linha(n_linha): optamos por esse campo para que o acesso do usuário sobre o sistema fique mais coerente com sua realidade.

Campo Tipo de ônibus (tipo_de_onibus): criamos esse campo para que haja mais informações sobre o ônibus para o usuário.

Ponto de ônibus:

Campo Número do ponto (n_ponto): serve para melhor indentificarmos cada ponto de ônibus, e ralacioná-lo com os números dos ônibus que ali passam.

Bairro, Cidade Estado:

Campo Código (codigo): criamos esse campo para que cada um tenha sua “identidade” assim não ocorre o risco de terem o mesmo nome.

Campo Nome (nome): criamos esse campo para que o usuário tenha melhor acesso sobre a informação.

Logradouro:

Campo Descrição (descricao): optamos por esse campo para saber o tipo de logradouro.

Campo Código (codigo):  criamos esse campo para que cada um tenha sua “identidade” assim não ocorre o risco de terem o mesmo nome.

Nome Logradouro:

Campo Nome (nome): optamos para o nome de cada logradouro, relacionando com o tabela Logradouro.

Relação Ponto Ônibus:

Campo Horário (horario): criamos esse campo para que tenhamos o horário em que cada ônibus passa em determinado ponto.

Campo Ordem (ordem): optamos por esse campo para sabermos a ordem em que os ônibus passam nos pontos.

Campo Id (id): optamos por esse campo para que a relação ônibus e ponto de ônibus tenham uma “identidade”.

Relação Ônibus e Usuário:

Campo Data (data): criamos esse campo para um melhor controle e organização sobre o sistema. 

Relação Ponto de Ônibus e Usuário:

Campo Data (data): criamos esse campo para um melhor controle e organização sobre o sistema.

    
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
   ![Modelo lógico](https://github.com/MDBD1/trabalho01/blob/master/imagens/%C3%BAltimomodelologico.png)
### 7 MODELO FÍSICO<br>

CREATE TABLE USUARIO (
    email varchar(80),
    senha varchar(80),
    nome varchar(80),
    n_da_casa int,
    codigo serial PRIMARY KEY
);

CREATE TABLE ONIBUS (
    n_onibus int PRIMARY KEY,
    n_linha int,
    itinerario varchar(255),
    tipo_de_onibus varchar(80)
);

CREATE TABLE PONTO_DE_ONIBUS (
    n_ponto int PRIMARY KEY
);

CREATE TABLE CIDADE (
    nome varchar(80),
    codigo int PRIMARY KEY,
    FK_ESTADO_codigo int
);

CREATE TABLE ESTADO (
    nome varchar(80),
    codigo int PRIMARY KEY
);

CREATE TABLE BAIRRO (
    nome varchar(80),
    codigo int PRIMARY KEY,
    FK_CIDADE_codigo int
);

CREATE TABLE LOGRADOURO (
    codigo int PRIMARY KEY,
    descricao varchar(255),
    FK_BAIRRO_codigo int
);

CREATE TABLE NOME_LOGRADOURO (
    nome varchar(255),
    FK_LOGRADOURO_codigo int
);

CREATE TABLE RELA_PONTO_ONIBUS_Relacao_1 (
    id serial PRIMARY KEY,
    horario time,
    ordem serial,
    fk_ONIBUS_n_onibus int,
    fk_PONTO_DE_ONIBUS_n_ponto int
);

CREATE TABLE usu_logradouro (
    fk_USUARIO_codigo serial,
    fk_LOGRADOURO_codigo int
);

CREATE TABLE ponto_logradouro (
    fk_LOGRADOURO_codigo int,
    fk_PONTO_DE_ONIBUS_n_ponto int
);

CREATE TABLE onibus_usuario (
    fk_USUARIO_codigo serial,
    fk_ONIBUS_n_onibus int,
    data DATE
);

CREATE TABLE ponto_usuario (
    fk_USUARIO_codigo serial,
    fk_PONTO_DE_ONIBUS_n_ponto int,
    data DATE
);
 
ALTER TABLE CIDADE ADD CONSTRAINT FK_CIDADE_2
    FOREIGN KEY (FK_ESTADO_codigo)
    REFERENCES ESTADO (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE BAIRRO ADD CONSTRAINT FK_BAIRRO_2
    FOREIGN KEY (FK_CIDADE_codigo)
    REFERENCES CIDADE (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE LOGRADOURO ADD CONSTRAINT FK_LOGRADOURO_2
    FOREIGN KEY (FK_BAIRRO_codigo)
    REFERENCES BAIRRO (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE NOME_LOGRADOURO ADD CONSTRAINT FK_NOME_LOGRADOURO_1
    FOREIGN KEY (FK_LOGRADOURO_codigo)
    REFERENCES LOGRADOURO (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE RELA_PONTO_ONIBUS_Relacao_1 ADD CONSTRAINT FK_RELA_PONTO_ONIBUS_Relacao_1_2
    FOREIGN KEY (fk_ONIBUS_n_onibus)
    REFERENCES ONIBUS (n_onibus);
 
ALTER TABLE RELA_PONTO_ONIBUS_Relacao_1 ADD CONSTRAINT FK_RELA_PONTO_ONIBUS_Relacao_1_3
    FOREIGN KEY (fk_PONTO_DE_ONIBUS_n_ponto)
    REFERENCES PONTO_DE_ONIBUS (n_ponto);
 
ALTER TABLE usu_logradouro ADD CONSTRAINT FK_usu_logradouro_1
    FOREIGN KEY (fk_USUARIO_codigo)
    REFERENCES USUARIO (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE usu_logradouro ADD CONSTRAINT FK_usu_logradouro_2
    FOREIGN KEY (fk_LOGRADOURO_codigo)
    REFERENCES LOGRADOURO (codigo)
    ON DELETE SET NULL;
 
ALTER TABLE ponto_logradouro ADD CONSTRAINT FK_ponto_logradouro_1
    FOREIGN KEY (fk_LOGRADOURO_codigo)
    REFERENCES LOGRADOURO (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE ponto_logradouro ADD CONSTRAINT FK_ponto_logradouro_2
    FOREIGN KEY (fk_PONTO_DE_ONIBUS_n_ponto)
    REFERENCES PONTO_DE_ONIBUS (n_ponto)
    ON DELETE RESTRICT;
 
ALTER TABLE onibus_usuario ADD CONSTRAINT FK_onibus_usuario_1
    FOREIGN KEY (fk_USUARIO_codigo)
    REFERENCES USUARIO (codigo)
    ON DELETE SET NULL;
 
ALTER TABLE onibus_usuario ADD CONSTRAINT FK_onibus_usuario_2
    FOREIGN KEY (fk_ONIBUS_n_onibus)
    REFERENCES ONIBUS (n_onibus)
    ON DELETE SET NULL;
 
ALTER TABLE ponto_usuario ADD CONSTRAINT FK_ponto_usuario_1
    FOREIGN KEY (fk_USUARIO_codigo)
    REFERENCES USUARIO (codigo)
    ON DELETE SET NULL;
 
ALTER TABLE ponto_usuario ADD CONSTRAINT FK_ponto_usuario_2
    FOREIGN KEY (fk_PONTO_DE_ONIBUS_n_ponto)
    REFERENCES PONTO_DE_ONIBUS (n_ponto)
    ON DELETE SET NULL;    
        
### 8 INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
#### 8.1 DETALHAMENTO DAS INFORMAÇÕES
        a) inclusão das instruções de inserção dos dados nas tabelas criadas pelo script de modelo físico
        b) formato .SQL
        
insert into RELA_PONTO_ONIBUS_Relacao_1(id, horario, ordem, fk_onibus_n_onibus. fk_ponto_de_onibus_n_ponto) values (234567,'20:09', 1, 234567, 128937),(534285,'12:08',12, 534285, 12345),(123454,'13:00', 7, 876557, 4893095),(876557,'05:50', 5, 785444, 123090),(645323,'04:00',53, 978678, 53034), (785444,'14:55',9, 64321, 96543),(45689,'09:05',10, 534285, 1006),(978678,'20:45',12, 234567, 87654),(12345,'23:50',123, 64321, 12456),(64321,'19:02',48, 785444, 87654);

insert into ponto_usuario(fk_usuario_codigo, fk_ponto_de_onibus_n_ponto, data) values ('1', 128937, '12-09-2018'), ('2', 12345, '10-10-2018'), ('3',87654, '09-11-2018'),('4', 57687,'04-09-2018'), ('5', 53034,'05-08-2018'), ('6', 96543,'08-11-2018'), ('7',1006 ,'07-11-2018'), ('8', 12456,'10-11-2018'), ('9', 123090,'10-10-2018'), ('10',4893095,'09-11-2018');

insert into onibus_usuario(fk_usuario_codigo, fk_onibus_n_onibus, data) values ('1',234567,'12-09-2018'), ('2',534285,'10-10-2018'), ('3',123454,'11-11-2018'),('4',876557,'09-09-2018'), ('5',645323,'05-08-2018'), ('6',785444,'09-11-2018'), ('7',45689,'10-11-2018'), ('8',978678,'10-11-2018'), ('9',12345,'10-10-2018'), ('10',64321,'11-11-2018');

insert into logradouro (codigo, descricao, fk_bairro_codigo) values (1, 'rua', 10), (2, 'avenida', 9), (3, 'alameda', 8), (4, 'ladeira', 7), (5, 'viaduto', 6), (6, 'canal', 5), (7, 'beco', 4), (8, 'contorno', 3), (9, 'trevo', 2), (10, 'via', 1);

insert into ponto_logradouro (fk_logradouro_codigo, fk_ponto_de_onibus_n_ponto) values (1, 128937), (2, 12345), (3, 87654), (4, 57687), (5, 53034), (6, 96543) (7, 1006), (8, 12456), (9, 123090), (10, 4893095);

insert into usu_logradouro (fk_usuario_codigo, fk_logradouro_codigo) values ('1', 2), ('2', 3), ('3', 4), ('4', 5), ('5', 6), ('6', 7), ('7', 8), ('8', 9), ('9', 10), ('10', 1);

insert into nome_logradouro (nome, fk_logradouro_codigo) values ('Rua Anchieta', 1), ('Avenida Fernando Ferrari', 2), ('Avenida Norte Sul', 2), ('Avenida Central', 2), ('Avenida Eudes Scherrer de Souza', 2), ('Civit ll', 2), ('Avenida João Palácio', 2), ('Avenida Américo Buiaz', 2), ('Avenida Guarapari', 2), ('Avenida Reta da Penha', 2);

insert into estado (nome, codigo) values ('Espírito Santo', 1), ('São Paulo', 2), ('Rio de Janeiro', 3), ('Bahia', 4), ('Minas Gerais', 5), ('Rio Grande do Sul', 6), ('Amazônia', 7), ('Ceará', 8), ('Mato Grosso', 9), ('Goiás', 10);

insert into cidade (nome, codigo, fk_estado_codigo) values ('Serra', 1, 1), ('Vitória', 2, 1), ('Vila Velha', 3, 1), ('Cariacica', 4, 1), ('Colatina', 5, 1), ('Viana', 6, 1), ('Salvador', 7, 4), ('Vitória da Conquista', 8, 4), ('Itapetinga', 9, 4), ('Fundão', 10, 1);

insert into bairro (nome, codigo, fk_cidade_codigo) values ('Manguinhos', 1, 1), ('Goiabeiras', 2, 2), ('Laranjeiras', 3, 1), ('Boa Vista', 4, 2), ('Itapina', 5, 5), ('Mata da Praia', 6, 2), ('Jardim Comburir', 7, 2), ('Jardim da Penha', 8, 2), ('Serra Cede', 9, 1), ('Jacaraípe', 10, 1);

insert into ponto_de_onibus(n_ponto) values (128937), (12345), (87654), (57687), (53034), (96543), (1006), (12456), (123090), (4893095);

insert into USUARIO(email,senha,nome, codigo, n_da_casa) values ('fernadasilva@email.com','tuyghj678','Fernanda da Silva','1','56'),('mariaclara@email.com','sckopdnefj8','Maria Clara dos Santos','2' ,'1600'),('robertaOliveira@email.com','qreytjukfd','Roberta Oliveira','3','1601'), ('dsgfdhsj@email.com','bibibibibi','Mark Pereira','4' ,'1602'), ('blablabla@email.com','qwer1234','Beatris dos Santos','5','1603'), ('lkdaqwe@email.com','123890iop','Jackson Wang','6','1604'), ('weakSempre@email.com','universo123','Karen Bachini','7','1605'), ('bliblipimpim@gmail','kkj1234','Maria Carolina Da Silva','8','1606'), ('guiSilveira@email.com','6543212','Guilherme Silveira','9','1607'), ('jubilix@gmail.com','coisalinda','Juliana Vasconcelos','10', '50');

insert into onibus(n_onibus,n_linha,itinerario, tipo_de_onibus) values (234567, 400, 'Avenida Paulo Pereira Gomes', 'transcol'),(534285, 500,'Rua Anchieta', 'transcol'), (123454, 567,'Avenida Fernando Ferrari', 'tabuazeiro'),(876557, 900,'Avenida Norte Sul', 'transcol'), (645323, 432,'Avenida Central', 'tabuazeiro'),(785444, 72,'Avenida Eudes Scherrer de Souza', 'tabuazeiro'), (45689, 789,'Civit ll', 'transcol'),(978678,500,'Avenida João Palácio', 'transcol'), (12345, 121,'Avenida Américo Buiaz', 'tabuazeiro'),(64321, 560,'Avenida Guarapari','transcol' );

<br>

#### 8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS<br>
        a) Junção dos scripts anteriores em um único script
        (create para tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL
        
CREATE TABLE USUARIO ( email varchar(80), senha varchar(80), nome varchar(80), n_da_casa int, codigo serial PRIMARY KEY );

CREATE TABLE ONIBUS ( n_onibus int PRIMARY KEY, n_linha int, itinerario varchar(255), tipo_de_onibus varchar(80) );

CREATE TABLE PONTO_DE_ONIBUS ( n_ponto int PRIMARY KEY );

CREATE TABLE CIDADE ( nome varchar(80), codigo int PRIMARY KEY, FK_ESTADO_codigo int );

CREATE TABLE ESTADO ( nome varchar(80), codigo int PRIMARY KEY );

CREATE TABLE BAIRRO ( nome varchar(80), codigo int PRIMARY KEY, FK_CIDADE_codigo int );

CREATE TABLE LOGRADOURO ( codigo int PRIMARY KEY, descricao varchar(255), FK_BAIRRO_codigo int );

CREATE TABLE NOME_LOGRADOURO ( nome varchar(255), FK_LOGRADOURO_codigo int );

CREATE TABLE RELA_PONTO_ONIBUS_Relacao_1 ( id serial PRIMARY KEY, horario time, ordem serial, fk_ONIBUS_n_onibus int, fk_PONTO_DE_ONIBUS_n_ponto int );

CREATE TABLE usu_logradouro ( fk_USUARIO_codigo serial, fk_LOGRADOURO_codigo int );

CREATE TABLE ponto_logradouro ( fk_LOGRADOURO_codigo int, fk_PONTO_DE_ONIBUS_n_ponto int );

CREATE TABLE onibus_usuario ( fk_USUARIO_codigo serial, fk_ONIBUS_n_onibus int, data DATE );

CREATE TABLE ponto_usuario ( fk_USUARIO_codigo serial, fk_PONTO_DE_ONIBUS_n_ponto int, data DATE );

ALTER TABLE CIDADE ADD CONSTRAINT FK_CIDADE_2 FOREIGN KEY (FK_ESTADO_codigo) REFERENCES ESTADO (codigo) ON DELETE RESTRICT;

ALTER TABLE BAIRRO ADD CONSTRAINT FK_BAIRRO_2 FOREIGN KEY (FK_CIDADE_codigo) REFERENCES CIDADE (codigo) ON DELETE RESTRICT;

ALTER TABLE LOGRADOURO ADD CONSTRAINT FK_LOGRADOURO_2 FOREIGN KEY (FK_BAIRRO_codigo) REFERENCES BAIRRO (codigo) ON DELETE RESTRICT;

ALTER TABLE NOME_LOGRADOURO ADD CONSTRAINT FK_NOME_LOGRADOURO_1 FOREIGN KEY (FK_LOGRADOURO_codigo) REFERENCES LOGRADOURO (codigo) ON DELETE RESTRICT;

ALTER TABLE RELA_PONTO_ONIBUS_Relacao_1 ADD CONSTRAINT FK_RELA_PONTO_ONIBUS_Relacao_1_2 FOREIGN KEY (fk_ONIBUS_n_onibus) REFERENCES ONIBUS (n_onibus);

ALTER TABLE RELA_PONTO_ONIBUS_Relacao_1 ADD CONSTRAINT FK_RELA_PONTO_ONIBUS_Relacao_1_3 FOREIGN KEY (fk_PONTO_DE_ONIBUS_n_ponto) REFERENCES PONTO_DE_ONIBUS (n_ponto);

ALTER TABLE usu_logradouro ADD CONSTRAINT FK_usu_logradouro_1 FOREIGN KEY (fk_USUARIO_codigo) REFERENCES USUARIO (codigo) ON DELETE RESTRICT;

ALTER TABLE usu_logradouro ADD CONSTRAINT FK_usu_logradouro_2 FOREIGN KEY (fk_LOGRADOURO_codigo) REFERENCES LOGRADOURO (codigo) ON DELETE SET NULL;

ALTER TABLE ponto_logradouro ADD CONSTRAINT FK_ponto_logradouro_1 FOREIGN KEY (fk_LOGRADOURO_codigo) REFERENCES LOGRADOURO (codigo) ON DELETE RESTRICT;

ALTER TABLE ponto_logradouro ADD CONSTRAINT FK_ponto_logradouro_2 FOREIGN KEY (fk_PONTO_DE_ONIBUS_n_ponto) REFERENCES PONTO_DE_ONIBUS (n_ponto) ON DELETE RESTRICT;

ALTER TABLE onibus_usuario ADD CONSTRAINT FK_onibus_usuario_1 FOREIGN KEY (fk_USUARIO_codigo) REFERENCES USUARIO (codigo) ON DELETE SET NULL;

ALTER TABLE onibus_usuario ADD CONSTRAINT FK_onibus_usuario_2 FOREIGN KEY (fk_ONIBUS_n_onibus) REFERENCES ONIBUS (n_onibus) ON DELETE SET NULL;

ALTER TABLE ponto_usuario ADD CONSTRAINT FK_ponto_usuario_1 FOREIGN KEY (fk_USUARIO_codigo) REFERENCES USUARIO (codigo) ON DELETE SET NULL;

ALTER TABLE ponto_usuario ADD CONSTRAINT FK_ponto_usuario_2 FOREIGN KEY (fk_PONTO_DE_ONIBUS_n_ponto) REFERENCES PONTO_DE_ONIBUS (n_ponto) ON DELETE SET NULL;

insert into RELA_PONTO_ONIBUS_Relacao_1(id, horario, ordem, fk_onibus_n_onibus. fk_ponto_de_onibus_n_ponto) values (234567,'20:09', 1, 234567, 128937),(534285,'12:08',12, 534285, 12345),(123454,'13:00', 7, 876557, 4893095),(876557,'05:50', 5, 785444, 123090),(645323,'04:00',53, 978678, 53034), (785444,'14:55',9, 64321, 96543),(45689,'09:05',10, 534285, 1006),(978678,'20:45',12, 234567, 87654),(12345,'23:50',123, 64321, 12456),(64321,'19:02',48, 785444, 87654);

insert into ponto_usuario(fk_usuario_codigo, fk_ponto_de_onibus_n_ponto, data) values ('1', 128937, '12-09-2018'), ('2', 12345, '10-10-2018'), ('3',87654, '09-11-2018'),('4', 57687,'04-09-2018'), ('5', 53034,'05-08-2018'), ('6', 96543,'08-11-2018'), ('7',1006 ,'07-11-2018'), ('8', 12456,'10-11-2018'), ('9', 123090,'10-10-2018'), ('10',4893095,'09-11-2018');

insert into onibus_usuario(fk_usuario_codigo, fk_onibus_n_onibus, data) values ('1',234567,'12-09-2018'), ('2',534285,'10-10-2018'), ('3',123454,'11-11-2018'),('4',876557,'09-09-2018'), ('5',645323,'05-08-2018'), ('6',785444,'09-11-2018'), ('7',45689,'10-11-2018'), ('8',978678,'10-11-2018'), ('9',12345,'10-10-2018'), ('10',64321,'11-11-2018');

insert into logradouro (codigo, descricao, fk_bairro_codigo) values (1, 'rua', 10), (2, 'avenida', 9), (3, 'alameda', 8), (4, 'ladeira', 7), (5, 'viaduto', 6), (6, 'canal', 5), (7, 'beco', 4), (8, 'contorno', 3), (9, 'trevo', 2), (10, 'via', 1);

insert into ponto_logradouro (fk_logradouro_codigo, fk_ponto_de_onibus_n_ponto) values (1, 128937), (2, 12345), (3, 87654), (4, 57687), (5, 53034), (6, 96543) (7, 1006), (8, 12456), (9, 123090), (10, 4893095);

insert into usu_logradouro (fk_usuario_codigo, fk_logradouro_codigo) values ('1', 2), ('2', 3), ('3', 4), ('4', 5), ('5', 6), ('6', 7), ('7', 8), ('8', 9), ('9', 10), ('10', 1);

insert into nome_logradouro (nome, fk_logradouro_codigo) values ('Rua Anchieta', 1), ('Avenida Fernando Ferrari', 2), ('Avenida Norte Sul', 2), ('Avenida Central', 2), ('Avenida Eudes Scherrer de Souza', 2), ('Civit ll', 2), ('Avenida João Palácio', 2), ('Avenida Américo Buiaz', 2), ('Avenida Guarapari', 2), ('Avenida Reta da Penha', 2);

insert into estado (nome, codigo) values ('Espírito Santo', 1), ('São Paulo', 2), ('Rio de Janeiro', 3), ('Bahia', 4), ('Minas Gerais', 5), ('Rio Grande do Sul', 6), ('Amazônia', 7), ('Ceará', 8), ('Mato Grosso', 9), ('Goiás', 10);

insert into cidade (nome, codigo, fk_estado_codigo) values ('Serra', 1, 1), ('Vitória', 2, 1), ('Vila Velha', 3, 1), ('Cariacica', 4, 1), ('Colatina', 5, 1), ('Viana', 6, 1), ('Salvador', 7, 4), ('Vitória da Conquista', 8, 4), ('Itapetinga', 9, 4), ('Fundão', 10, 1);

insert into bairro (nome, codigo, fk_cidade_codigo) values ('Manguinhos', 1, 1), ('Goiabeiras', 2, 2), ('Laranjeiras', 3, 1), ('Boa Vista', 4, 2), ('Itapina', 5, 5), ('Mata da Praia', 6, 2), ('Jardim Comburir', 7, 2), ('Jardim da Penha', 8, 2), ('Serra Cede', 9, 1), ('Jacaraípe', 10, 1);

insert into ponto_de_onibus(n_ponto) values (128937), (12345), (87654), (57687), (53034), (96543), (1006), (12456), (123090), (4893095);

insert into USUARIO(email,senha,nome, codigo, n_da_casa) values ('fernadasilva@email.com','tuyghj678','Fernanda da Silva','1','56'),('mariaclara@email.com','sckopdnefj8','Maria Clara dos Santos','2' ,'1600'),('robertaOliveira@email.com','qreytjukfd','Roberta Oliveira','3','1601'), ('dsgfdhsj@email.com','bibibibibi','Mark Pereira','4' ,'1602'), ('blablabla@email.com','qwer1234','Beatris dos Santos','5','1603'), ('lkdaqwe@email.com','123890iop','Jackson Wang','6','1604'), ('weakSempre@email.com','universo123','Karen Bachini','7','1605'), ('bliblipimpim@gmail','kkj1234','Maria Carolina Da Silva','8','1606'), ('guiSilveira@email.com','6543212','Guilherme Silveira','9','1607'), ('jubilix@gmail.com','coisalinda','Juliana Vasconcelos','10', '50');

insert into onibus(n_onibus,n_linha,itinerario, tipo_de_onibus) values (234567, 400, 'Avenida Paulo Pereira Gomes', 'transcol'),(534285, 500,'Rua Anchieta', 'transcol'), (123454, 567,'Avenida Fernando Ferrari', 'tabuazeiro'),(876557, 900,'Avenida Norte Sul', 'transcol'), (645323, 432,'Avenida Central', 'tabuazeiro'),(785444, 72,'Avenida Eudes Scherrer de Souza', 'tabuazeiro'), (45689, 789,'Civit ll', 'transcol'),(978678,500,'Avenida João Palácio', 'transcol'), (12345, 121,'Avenida Américo Buiaz', 'tabuazeiro'),(64321, 560,'Avenida Guarapari','transcol' );


<br>
        
#### 8.3 INCLUSÃO DO SCRIPT PARA EXCLUSÃO DE TABELAS EXISTENTES, CRIAÇÃO DE TABELA NOVAS E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script
        (Drop table + Create de tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL
  
        
drop table usuario; 
</br>
drop table ponto_onibus;
</br>
drop table onibus;
</br>
drop table logradouro;
</br>
drop table nome_logradouro;
</br>
drop table bairro;
</br>
drop table estado;
</br>
drop table cidade;
</br>
drop table onibus_usuario;
</br>
drop table ponto_usuario;
</br>
drop table usu_logradouro;
</br>
drop table rela_ponto_onibus_relacao_1;
</br>
drop table ponto_logradouro;
</br>


CREATE TABLE USUARIO (
    email varchar(80),
    senha varchar(80),
    nome varchar(80),
    n_da_casa int,
    codigo serial PRIMARY KEY
);

CREATE TABLE ONIBUS (
    n_onibus int PRIMARY KEY,
    n_linha int,
    tipo_de_onibus varchar(80)
);

CREATE TABLE PONTO_DE_ONIBUS (
    n_ponto int PRIMARY KEY
);

CREATE TABLE CIDADE (
    nome varchar(80),
    codigo int PRIMARY KEY,
    FK_ESTADO_codigo int
);

CREATE TABLE ESTADO (
    nome varchar(80),
    codigo int PRIMARY KEY
);

CREATE TABLE BAIRRO (
    nome varchar(80),
    codigo int PRIMARY KEY,
    FK_CIDADE_codigo int
);

CREATE TABLE LOGRADOURO (
    codigo int PRIMARY KEY,
    descricao varchar(255),
    FK_BAIRRO_codigo int
);

CREATE TABLE NOME_LOGRADOURO (
    nome varchar(255),
    FK_LOGRADOURO_codigo int
);

CREATE TABLE RELA_PONTO_ONIBUS_Relação_1 (
    id serial PRIMARY KEY,
    horario time,
    ordem serial,
    fk_ONIBUS_n_onibus int,
    fk_PONTO_DE_ONIBUS_n_ponto int
);

CREATE TABLE usu_logradouro (
    fk_USUARIO_codigo serial,
    fk_LOGRADOURO_codigo int
);

CREATE TABLE ponto_logradouro (
    fk_LOGRADOURO_codigo int,
    fk_PONTO_DE_ONIBUS_n_ponto int
);

CREATE TABLE onibus_usuario (
    fk_USUARIO_codigo serial,
    fk_ONIBUS_n_onibus int,
    data DATE
);

CREATE TABLE ponto_usuario (
    fk_USUARIO_codigo serial,
    fk_PONTO_DE_ONIBUS_n_ponto int,
    data DATE
);
 
ALTER TABLE CIDADE ADD CONSTRAINT FK_CIDADE_2
    FOREIGN KEY (FK_ESTADO_codigo)
    REFERENCES ESTADO (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE BAIRRO ADD CONSTRAINT FK_BAIRRO_2
    FOREIGN KEY (FK_CIDADE_codigo)
    REFERENCES CIDADE (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE LOGRADOURO ADD CONSTRAINT FK_LOGRADOURO_2
    FOREIGN KEY (FK_BAIRRO_codigo)
    REFERENCES BAIRRO (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE NOME_LOGRADOURO ADD CONSTRAINT FK_NOME_LOGRADOURO_1
    FOREIGN KEY (FK_LOGRADOURO_codigo)
    REFERENCES LOGRADOURO (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE RELA_PONTO_ONIBUS_Relação_1 ADD CONSTRAINT FK_RELA_PONTO_ONIBUS_Relação_1_2
    FOREIGN KEY (fk_ONIBUS_n_onibus)
    REFERENCES ONIBUS (n_onibus);
 
ALTER TABLE RELA_PONTO_ONIBUS_Relação_1 ADD CONSTRAINT FK_RELA_PONTO_ONIBUS_Relação_1_3
    FOREIGN KEY (fk_PONTO_DE_ONIBUS_n_ponto)
    REFERENCES PONTO_DE_ONIBUS (n_ponto);
 
ALTER TABLE usu_logradouro ADD CONSTRAINT FK_usu_logradouro_1
    FOREIGN KEY (fk_USUARIO_codigo)
    REFERENCES USUARIO (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE usu_logradouro ADD CONSTRAINT FK_usu_logradouro_2
    FOREIGN KEY (fk_LOGRADOURO_codigo)
    REFERENCES LOGRADOURO (codigo)
    ON DELETE SET NULL;
 
ALTER TABLE ponto_logradouro ADD CONSTRAINT FK_ponto_logradouro_1
    FOREIGN KEY (fk_LOGRADOURO_codigo)
    REFERENCES LOGRADOURO (codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE ponto_logradouro ADD CONSTRAINT FK_ponto_logradouro_2
    FOREIGN KEY (fk_PONTO_DE_ONIBUS_n_ponto)
    REFERENCES PONTO_DE_ONIBUS (n_ponto)
    ON DELETE RESTRICT;
 
ALTER TABLE onibus_usuario ADD CONSTRAINT FK_onibus_usuario_1
    FOREIGN KEY (fk_USUARIO_codigo)
    REFERENCES USUARIO (codigo)
    ON DELETE SET NULL;
 
ALTER TABLE onibus_usuario ADD CONSTRAINT FK_onibus_usuario_2
    FOREIGN KEY (fk_ONIBUS_n_onibus)
    REFERENCES ONIBUS (n_onibus)
    ON DELETE SET NULL;
 
ALTER TABLE ponto_usuario ADD CONSTRAINT FK_ponto_usuario_1
    FOREIGN KEY (fk_USUARIO_codigo)
    REFERENCES USUARIO (codigo)
    ON DELETE SET NULL;
 
ALTER TABLE ponto_usuario ADD CONSTRAINT FK_ponto_usuario_2
    FOREIGN KEY (fk_PONTO_DE_ONIBUS_n_ponto)
    REFERENCES PONTO_DE_ONIBUS (n_ponto)
    ON DELETE SET NULL;


insert into RELA_PONTO_ONIBUS_Relacao_1(id, horario, ordem, fk_onibus_n_onibus. fk_ponto_de_onibus_n_ponto) values (234567,'20:09', 1, 234567, 128937),(534285,'12:08',12, 534285, 12345),(123454,'13:00', 7, 876557, 4893095),(876557,'05:50', 5, 785444, 123090),(645323,'04:00',53, 978678, 53034), (785444,'14:55',9, 64321, 96543),(45689,'09:05',10, 534285, 1006),(978678,'20:45',12, 234567, 87654),(12345,'23:50',123, 64321, 12456),(64321,'19:02',48, 785444, 87654);

insert into ponto_usuario(fk_usuario_codigo, fk_ponto_de_onibus_n_ponto, data) values ('1', 128937, '12-09-2018'), ('2', 12345, '10-10-2018'), ('3',87654, '09-11-2018'),('4', 57687,'04-09-2018'), ('5', 53034,'05-08-2018'), ('6', 96543,'08-11-2018'), ('7',1006 ,'07-11-2018'), ('8', 12456,'10-11-2018'), ('9', 123090,'10-10-2018'), ('10',4893095,'09-11-2018');

insert into onibus_usuario(fk_usuario_codigo, fk_onibus_n_onibus, data) values ('1',234567,'12-09-2018'), ('2',534285,'10-10-2018'), ('3',123454,'11-11-2018'),('4',876557,'09-09-2018'), ('5',645323,'05-08-2018'), ('6',785444,'09-11-2018'), ('7',45689,'10-11-2018'), ('8',978678,'10-11-2018'), ('9',12345,'10-10-2018'), ('10',64321,'11-11-2018');

insert into logradouro (codigo, descricao, fk_bairro_codigo) values (1, 'rua', 10), (2, 'avenida', 9), (3, 'alameda', 8), (4, 'ladeira', 7), (5, 'viaduto', 6), (6, 'canal', 5), (7, 'beco', 4), (8, 'contorno', 3), (9, 'trevo', 2), (10, 'via', 1);

insert into ponto_logradouro (fk_logradouro_codigo, fk_ponto_de_onibus_n_ponto) values (1, 128937), (2, 12345), (3, 87654), (4, 57687), (5, 53034), (6, 96543) (7, 1006), (8, 12456), (9, 123090), (10, 4893095);

insert into usu_logradouro (fk_usuario_codigo, fk_logradouro_codigo) values ('1', 2), ('2', 3), ('3', 4), ('4', 5), ('5', 6), ('6', 7), ('7', 8), ('8', 9), ('9', 10), ('10', 1);

insert into nome_logradouro (nome, fk_logradouro_codigo) values ('Rua Anchieta', 1), ('Avenida Fernando Ferrari', 2), ('Avenida Norte Sul', 2), ('Avenida Central', 2), ('Avenida Eudes Scherrer de Souza', 2), ('Civit ll', 2), ('Avenida João Palácio', 2), ('Avenida Américo Buiaz', 2), ('Avenida Guarapari', 2), ('Avenida Reta da Penha', 2);

insert into estado (nome, codigo) values ('Espírito Santo', 1), ('São Paulo', 2), ('Rio de Janeiro', 3), ('Bahia', 4), ('Minas Gerais', 5), ('Rio Grande do Sul', 6), ('Amazônia', 7), ('Ceará', 8), ('Mato Grosso', 9), ('Goiás', 10);

insert into cidade (nome, codigo, fk_estado_codigo) values ('Serra', 1, 1), ('Vitória', 2, 1), ('Vila Velha', 3, 1), ('Cariacica', 4, 1), ('Colatina', 5, 1), ('Viana', 6, 1), ('Salvador', 7, 4), ('Vitória da Conquista', 8, 4), ('Itapetinga', 9, 4), ('Fundão', 10, 1);

insert into bairro (nome, codigo, fk_cidade_codigo) values ('Manguinhos', 1, 1), ('Goiabeiras', 2, 2), ('Laranjeiras', 3, 1), ('Boa Vista', 4, 2), ('Itapina', 5, 5), ('Mata da Praia', 6, 2), ('Jardim Comburir', 7, 2), ('Jardim da Penha', 8, 2), ('Serra Cede', 9, 1), ('Jacaraípe', 10, 1);

insert into ponto_de_onibus(n_ponto) values (128937), (12345), (87654), (57687), (53034), (96543), (1006), (12456), (123090), (4893095);

insert into USUARIO(email,senha,nome, codigo, n_da_casa) values ('fernadasilva@email.com','tuyghj678','Fernanda da Silva','1','56'),('mariaclara@email.com','sckopdnefj8','Maria Clara dos Santos','2' ,'1600'),('robertaOliveira@email.com','qreytjukfd','Roberta Oliveira','3','1601'), ('dsgfdhsj@email.com','bibibibibi','Mark Pereira','4' ,'1602'), ('blablabla@email.com','qwer1234','Beatris dos Santos','5','1603'), ('lkdaqwe@email.com','123890iop','Jackson Wang','6','1604'), ('weakSempre@email.com','universo123','Karen Bachini','7','1605'), ('bliblipimpim@gmail','kkj1234','Maria Carolina Da Silva','8','1606'), ('guiSilveira@email.com','6543212','Guilherme Silveira','9','1607'), ('jubilix@gmail.com','coisalinda','Juliana Vasconcelos','10', '50');

insert into onibus(n_onibus,n_linha,itinerario, tipo_de_onibus) values (234567, 400, 'Avenida Paulo Pereira Gomes', 'transcol'),(534285, 500,'Rua Anchieta', 'transcol'), (123454, 567,'Avenida Fernando Ferrari', 'tabuazeiro'),(876557, 900,'Avenida Norte Sul', 'transcol'), (645323, 432,'Avenida Central', 'tabuazeiro'),(785444, 72,'Avenida Eudes Scherrer de Souza', 'tabuazeiro'), (45689, 789,'Civit ll', 'transcol'),(978678,500,'Avenida João Palácio', 'transcol'), (12345, 121,'Avenida Américo Buiaz', 'tabuazeiro'),(64321, 560,'Avenida Guarapari','transcol' );


<br>  
  
  
### 9 TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1 CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>

select * from usuario;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Usuario.png)<br>

select * from onibus;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/onibus.png)<br>

select * from ponto_de_onibus;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Ponto_de_Onibus.png)<br>

select * from rela_ponto_onibus_relacao_1;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Rela_onibus_ponto.png)<br>

select * from ponto_usuario;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Ponto_Usuario.png)<br>

select * from onibus_usuario;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Onibus_Usuario.png)<br>

select * from usu_logradouro;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Usu_Logradouro.png)<br>

select * from ponto_logradouro;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Ponto_Logradouro.png)<br>

select * from nome_logradouro;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Nome_Logradouro.png)<br>

select * from logradouro;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Logradouro.png)<br>

select * from estado;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Estado.png)<br>

select * from cidade;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Cidade.png)<br>

select * from bairro;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/Bairro.png)<br>
<br>

#### 9.2 CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>


![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/where1.png)<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/where2.png)<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/where3.png)<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/where4.png)<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/where5.png)<br>

<br>

#### 9.3 CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)<br>
  
    
a)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/1where.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/2where.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/3where.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/4where.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/5where.png)<br>

<br>

b)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/1.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/2.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/3.png)<br>

<br>
c)



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/11.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/22.png)<br>


![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/33.png)<br>

<br>
#### 9.4 CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12)<br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.


a)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/11.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/1where.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/where1.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/like1.png)<br>



![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/like2.png)<br>


<br>

b)<br>

Nós não fizemos esse tópico, pois o nosso trabalho não precisa da informação data.

<br>

#### 9.5 ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>

update usuario set nome='Júlia Ferreira' where senha='coisalinda';<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/9.5update1.png)<br>

update onibus set saida='11:00:00' where itinerario='Avenida Guarapari';<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/9.5update2.png)<br>

update ponto_de_onibus set tipo_de_onibus='Seletivo' where n_ponto=12345;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/9.5update3.png)<br>


ALTER TABLE acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS drop constraint FK_acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS_0;
ALTER TABLE acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS drop constraint FK_acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS_1;
ALTER TABLE acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS drop constraint FK_acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS_2;
ALTER TABLE ponto_onibus drop constraint FK_ponto_onibus_0;
ALTER TABLE ponto_onibus drop constraint FK_ponto_onibus_1;

ALTER TABLE acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS ADD CONSTRAINT FK_acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS_0
    FOREIGN KEY (FK_USUARIO_email)
    REFERENCES USUARIO (email)
    ON DELETE CASCADE ON UPDATE CASCADE;
 
ALTER TABLE acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS ADD CONSTRAINT FK_acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS_1
    FOREIGN KEY (FK_PONTO_DE_ONIBUS_n_ponto)
    REFERENCES PONTO_DE_ONIBUS (n_ponto)
    ON DELETE CASCADE ON UPDATE CASCADE;
 
ALTER TABLE acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS ADD CONSTRAINT FK_acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS_2
    FOREIGN KEY (FK_ONIBUS_n_onibus)
    REFERENCES ONIBUS (n_onibus)
    ON DELETE CASCADE ON UPDATE CASCADE;
 
ALTER TABLE ponto_onibus ADD CONSTRAINT FK_ponto_onibus_0
    FOREIGN KEY (FK_ONIBUS_n_onibus)
    REFERENCES ONIBUS (n_onibus)
    ON DELETE CASCADE ON UPDATE CASCADE;
 
ALTER TABLE ponto_onibus ADD CONSTRAINT FK_ponto_onibus_1
    FOREIGN KEY (FK_PONTO_DE_ONIBUS_n_ponto)
    REFERENCES PONTO_DE_ONIBUS (n_ponto)
    ON DELETE CASCADE ON UPDATE CASCADE; 

delete from usuario where n_da_casa='56';<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/9.5delete1.png)<br>

delete from onibus where n_onibus=234567;<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/9.5delete2.png)<br>

delete from ponto_de_onibus where bairro='Rosário de Fátima';<br>

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/9.5delete3.png)<br>
<br>
#### 9.6 CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br>
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
        
a)<br>
select U.nome,AU.FK_USUARIO_email,O.n_onibus, PDO.tipo_de_onibus, PO.FK_PONTO_DE_ONIBUS_n_ponto  from usuario U
inner join onibus O on(U.rua_avenida = O.itinerario)
inner join ponto_de_onibus 	PDO on (O.itinerario = PDO.rua_avenida)
inner join ponto_onibus PO on (PDO.n_ponto=PO.FK_PONTO_DE_ONIBUS_n_ponto)
inner join acesso_USUARIO_PONTO_DE_ONIBUS_ENTRADA_ONIBUS AU on (U.email = AU.FK_USUARIO_email);

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/9.6selecta.png)<br>

<br>
b)<br>

select U.nome,O.n_onibus, PDO.tipo_de_onibus  from usuario U
inner join onibus O on(U.rua_avenida = O.itinerario)
inner join ponto_de_onibus 	PDO on (O.itinerario = PDO.rua_avenida);

![Alt text](https://github.com/MDBD1/trabalho01/blob/master/imagens/9.6selectb.png)<br>

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


        
        


    





