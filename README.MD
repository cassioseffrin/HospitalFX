create database hospital

use hospital



create table paciente(
	id_paciente int auto_increment not null,
	nome_paciente varchar(50) not null,
	rg_paciente int not null,  
	cpf_paciente int not null, 
	sexo_paciente varchar(10) not null,
	dataNascimento_paciente date not null,
	telefone_paciente int,
	gravidade int,
	primary key(id_paciente)
)



create table medico(
	
	id_medico int auto_increment not null,
    
	nome_medico varchar(50) not null,
    
	rg_medico int not null,
    
	cpf_medico int not null,
    
	sexo_medico varchar(10) not null,
   
	dataNascimento_medico date not null,
    
	telefone_medico int,
    
	especialidade varchar(25),
    
	primary key(id_medico)

)



create table enfermeiro(
	
	id_enfermeiro int auto_increment not null,
   
	nome_enfermeiro varchar(50) not null,
    
	rg_enfermeiro int not null,
    
	cpf_enfermeiro int not null,
    
	sexo_enfermeiro varchar(10) not null,
    
	dataNascimento_enfermeiro date not null,
    
	telefone_enfermeiro int,
    
	dataAdmissao date not null,
    
	primary key(id_enfermeiro)

)



create table agenda(
	
	id_agenda int auto_increment not null,
    
	data_agenda date not null,
    
	horario varchar(10) not null,
    
	paciente varchar(50) not null,
   
	primary key(id_agenda)

)