Execute in conda env python 3.7.16 : 
```
conda create --name Steg python=3.7.16
conda activate Steg
pip install -r ai-server-requirements.txt
Edit path in ai-server-make-activate.cmd and ai-server-validate-activate.cmd
```

Execute in conda env python 3.11 :
```
conda create --name LOGIN python=3.11
conda activate LOGIN
pip install -r login-server-requirements.txt
Edit path in login-server-activate.cmd
```

Extract utils.rar into server folder : 
```
https://drive.google.com/file/d/1XeH8IrYYcyD4Ks-jbC4H2Mg7ZggoPav5/view?usp=sharing
```

In MYSQL Workbench
```
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'root';

create database mini_project;

use mini_project;

CREATE TABLE client_credentials (
    id INT AUTO_INCREMENT,
    email VARCHAR(255) NOT NULL,
    password VARCHAR(255) NOT NULL,
    company_name VARCHAR(255) NOT NULL,
    uid VARCHAR(255) NOT NULL,
    PRIMARY KEY (id),
    UNIQUE (email),
    UNIQUE (uid)
);
```
In frontend : 
```
npm i
npm start
```
Papers to read
```
https://arxiv.org/pdf/1904.05343
```
