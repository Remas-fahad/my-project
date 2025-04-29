-- create database tvtc ;
__________________________________________
create table dep (
depno int primary key ,
depname varchar(20) 
);
__________________________________________
create table std (
stdno int primary key ,
stdname varchar(20) ,
depno int ,
foreign key (depno) references dep(depno) );
___________________________________________
drop table dep ;
drop table std ;
alter table dep add loc varchar(20);
alter table dep drop column loc ;
alter table dep modify depname nvarchar(30);


SQL> alter table dep modify depname 



table DEP altered.

Elapsed: 00:00:00.015
