Install Minio
-------------

**Setup**
  
    kubectl apply -f resources/   
  
    helm upgrade --install minio minio \
      --namespace minio \
      --repo https://helm.min.io \
      --values values-minio.yaml
      
**Teardown**

    helm delete minio --namespace minio
    
    kubectl delete -f resources/