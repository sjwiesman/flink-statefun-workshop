Install Minio
-------------

**Setup**
  
    kubectl apply -f resources/
    
    helm install kafka \
        --namespace kafka-ca1 \
        -f values-kafka.yaml incubator/kafka 

**Teardown**

    helm delete kafka --namespace kafka-ca1
    
    kubectl delete -f resources/
    

