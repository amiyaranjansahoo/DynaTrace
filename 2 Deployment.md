#### How to deploy OneAgent to k8s cluster

### How to install helm
```sh
wget https://get.helm.sh/helm-v3.12.3-linux-amd64.tar.gz
tar -xzf helm-v3.12.3-linux-amd64.tar.gz
sudo mv ./linux-amd64/helm /usr/local/bin/
```

### Deploy the OneAgent
```sh
helm install dynatrace-operator oci://public.ecr.aws/dynatrace/dynatrace-operator \
    --create-namespace \
    --namespace dynatrace \
    --atomic
kubectl apply -f dynakube.yaml
```
