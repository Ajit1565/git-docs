#===================create new Database Postgres====================#

sudo -u postgres psql

"check version postgres"
select version();

"connection info of database"
\conninfo



﻿create new database db_name; 
grant all privileges on database mydb to myuser;

#### new user create for database roll assign
create user myuser with encrypted password 'mypass';

####### get backup for database     #########################

pg_dump -h localhost -U username database_name > new_databse_name.sql


#####select database#############
\c db_name




####========= setup scp=============================####

sudo apt install openssh-server

sudo scp example.zip username@192.168.42.62:Desktop




######============= git commands basic =====================##########
touch .gitignore
git init
git commit -m "Added gitignore file"
git remote add origin https://github.com/demo/hello.git
git push -u origin master


git status
git add .gitignore
git commit -m "Added gitignore file"
git push -u origin master


./subl

git status
git commit .gitignore -m "Added exception files"
git push -u origin master
git status


git add .
git status
git commit -m "push code"
git status
git push origin master








#########==========  Python django ==================###########

pip install virtualenv
pip -m venv mvenv


virtualenv mvenv --python==python3

source mvenv/bin/activate






##########==================== vim editer commands ======================================###########

sudo apt install vim


"For open file in terminal"
vi setting.py


"saving file without change write n file"
:q!


"saving contents in file => press Esc button for normal model"
:wq! or :x!

"just into on line number as 2 line number"
:2

"jump on last line of file"
:$

"delete line by dd key"
dd

"undo  or recovered delete items pres u"
u

" seleted or delete code by press v and after up and down arrow key"
v 


" for serach text"
:/hello


##############======================== end ======================############################


###############====================== Start nophup ================#######################

sudo ufw allow 8002
nohup python manage.py runserver 0.0.0.0:8002 $














