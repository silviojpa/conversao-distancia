# conversao-distancia

- Curso Desafio DevOps & Cloud (Aula 1 - Docker)

# Obs
- Todo processo necessário para gerenciar o container vai ser orquestrado pela image python

# dicas
-------------------------------------------------
- docker build -t conversao-distancia -f Dockerfile .
- docker run -d -p 8181:5000 conversao-distancia #exemplo de porta utilizada 8181 para porta do containar 5000
- docker login
- docker build -t silvio69luiz/conversao-distancia:v1 .
---------------------------------------------------
