# employee_vauxxo_request
CREATE DATABASE employee_employee

CREATE TABLE employee (
id INT PRIMARY KEY NOT NULL,
first name VARCHAR(15),
last name VARCHAR(15)
iddep INT, 
CONTRAINT FK_EMPLOYEE_IDDEP FOREIGN KEY (iddep) REFERENCES employee_departament (id)
                      );
                    
CREATE TABLE employee_departament (
id INT PRIMARY KEY NOT NULL,
name VARCHAR(25),
description VARCHAR(100)
                      );
                    
INSERT INTO employee_departament (id, name, description)
VALUES (201,'recursos humanos','contratacion de personal')
       (202,'direccion ejecutiva','toma las decisiones finales')
       (203,'mercadotecnia','todo el mercadeo de la empresa')
       (204,'administracion','gestiona los proyectos')
       (205,'innovacion','generan ideas acerca de proyectos nuevos')
       (206,'contaduria','lleva el control economico de la empresa');

INSERT INTO employee (id, first name, last name, iddep)
VALUES (101,'carlos','gonzalez',202),
       (102,'juan','perez',202),
       (103'pedro','lopez',205),
       (104,'jorge','martinez',205);

