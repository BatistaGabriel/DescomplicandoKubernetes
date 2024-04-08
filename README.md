# Descomplicando o Kubernetes

Este repositório foi criado para ter todos os materiais deste módulo do curso do [PICK 2024](https://www.linuxtips.io/pick)

## Comandos

### Rollout

#### Undo Latest

Para reverter um apply, podemos executar o seguinte comando:

```bash
k rollout undo deployment -n <namespace> <deployment name>
```

#### History

Para ver as revisões de um deployment, podemos executar o comando:
```bash
k rollout history deployment -n <namespace> <deployment name>
```

Para ver detalhes de um revisão específica, podemos executar o comando:

```bash
k rollout history deployment -n <namespace> <deployment name> --revision <revision number>
```

#### Pause/Resume Deployment

Caso seja necessário pausar o processo de um deployment, podemos executar o comando:

```bash
k rollout pause deployment -n <namespace> <deployment name>
```

Para volta a executar, podemos usar o comando:

```bash
k rollout resume deployment -n <namespace> <deployment name>
```

#### Rollback

Para reverter para uma revision específica, podemos executar o comando:

```bash
k rollout undo deployment -n <namespace> <deployment name> --to-revision=<revision number>
```

