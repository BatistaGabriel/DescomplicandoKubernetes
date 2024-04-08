# Descomplicando o Kubernetes

Este repositório foi criado para ter todos os materiais deste módulo do curso do [PICK 2024](https://www.linuxtips.io/pick)

## Comandos

### Rollout

Para reverter um apply, podemos executar o seguinte comando:

```bash
k rollout undo deployment -n <namespace> <deployment name>
```

Para ver as revisões de um deployment, podemos executar o comando:
```bash
k rollout history deployment -n <namespace> <deployment name>
```

Para ver detalhes de um revisão específica, podemos executar o comando:

```bash
k rollout history deployment -n <namespace> <deployment name> --revision <revision number>
```

