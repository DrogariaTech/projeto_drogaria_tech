# Projeto-ADS-4-Semestre
Projeto Drogaria Tech realizado no 4º semestre na UC de "Sistemas distribuídos e mobile".

Observaçoes do commit:
Quando utilizar o Docker/Kubernetes:
 1. Fazer: docker build -t *nome Dockerhub*/*microserviço* .  no terminal da pasta de cada microsserviço;
    1.1. Depois, ainda em cada pasta, fazer: docker push *nome Dockerhub*/*microserviço* ;
 2. Em um terminal para a pasta implantacao/kubernetes, fazer o código: kubectl apply -f *nome do arquivo*
    2.1. Fazer o mesmo código para todos os arquivos da pasta;
    2.2. Para checkar se os deployments/pods e services estão no ar, usar: kubectl get deployments, kubectl get pods, kubectl get services ;
    2.3. Pegar a porta gerada pelos services de arquivos focados em service e, no thunder client realizar get e post de cada serviço, tirando o barramento de eventos;
        2.3.1 http://localhost:*porta dada pelo service*/*microsserviço*
