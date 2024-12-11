## Setup Kind

- Instalação no Linux

```bash
curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.25.0/kind-linux-amd64
chmod +x ./kind
sudo mv ./kind /usr/local/bin/kind
```

- Criando um cluster

```bash
kind create cluster --name kind-argo --config kind-nodes.yaml
```

- Visualizar clusters

```bash
kind get clusters
```

- Visualizando nodes

```bash
kubectl get nodes
```

- Deletando Cluster

```bash
kind delete clusters
```

## Referência

- https://kind.sigs.k8s.io/docs/user/quick-start/