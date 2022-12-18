# Adote um aluno

This app is a landing page for a brazilian social project called ```adote um aluno``` and a control area for the leads. We are looking for students and teachers -or anyone who wants to contribute to expand the project.
## Server

The server is a very simple Flask server. Its dependencies are:

- Flask
- Flask SQLAlchemy
- SQLlite


MacOS
```
python3 -m venv venv

then loop throught: 
source venv/bin/activate
python server.py
```

## REST endpoints

The backend currently implements the following endpoints:
```
GET /alunos
GET /monitores
POST /alunos
POST /monitores
PATCH /monitor/{ID}
PATCH /aluno/{id}
DElETE /monitor/{ID}
DELETE /aluno/{id}
```

## Model definitions
Monitor

nome: number  
numero: string (required)  
exp: string  
created_at: number  
info: boolean

Aluno

nome: number  
numero: string (required)  
obj: string  
created_at: number  
info: boolean
