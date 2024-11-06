# conversao-distancia

- Curso Desafio DevOps & Cloud (Aula 1 - Docker)

# Obs
- Todo processo necessário para gerenciar o container vai ser orquestrado pela image python
- Ferramenta utilizada para LB em ON-PREMISE é Metal LB em Data Center

# dicas
----------------------- DOCKER --------------------------
- docker build -t conversao-distancia -f Dockerfile .
- docker run -d -p 8181:5000 conversao-distancia #exemplo de porta utilizada 8181 para porta do containar 5000
- docker login
- docker build -t silvio69luiz/conversao-distancia:v1 .
  
-----------------------KUBERNETES----------------------------
- k3d cluster create meucluster --servers 1 --agents 2
- kubectl get nodes
- kubectl apply -f k8s/deployment.yaml
- kubectl get pods
- kubectl describe pod "nome do pod"
- kubectl get replicaset
-  kubectl port-forward pod/NOME DO POD 8080:5000

Obs: Criação de LB local com NodePort 
- kubectl cluster create meucluster --servers 1 --agents 2 -p "8080:30000@loadbalancer"
 

