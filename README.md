# employee_vauxxo_request
CREATE DATABASE employee_employee

CREATE TABLE employee (
id_emp INT FOREIGN KEY,
first name VARCHAR(15),
last name VARCHAR(15)
                      );
CREATE TABLE employee_departament (
id_dep INT PRIMARY KEY,
name VARCHAR(25),
description VARCHAR(100)
                      );
                    
INSERT INTO employee (id, first name, last name)
VALUES (101,'carlos','gonzalez'),
       (102,'juan','perez'),
       (103'pedro','lopez'),
       (104,'jorge','martinez');

INSERT INTO employee_departament (id, name, description)
VALUES (201,'recursos humanos','contratacion de personal')
       (202,'direccion ejecutiva','toma las decisiones finales')
       (203,'mercadotecnia','todo el mercadeo de la empresa')
       (204,'administracion','gestiona los proyectos')
       (205,'innovacion','generan ideas acerca de proyectos nuevos')
       (206,'contaduria','lleva el control economico de la empresa');
       
ALTER TABLE employee_departament
ADD CONSTRAINT id_dep
FOREIGN KEY (id_emp) REFERENCES employee (id_emp)
go
