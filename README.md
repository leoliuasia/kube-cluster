# Create Kubernetes Cluster


## Step 1

```shell
ansible-playbook -i hosts initial.yml
```
## Step 2

```shell
ansible-playbook -i hosts kube-dependencies.yml

```

## Step 3

```shell
ansible-playbook -i hosts master.yml
```

## Step 4

```shell
ansible-playbook -i hosts workers.yml
```



# Reset kubernetes Cluster


```shell
ansible-playbook -i hosts reset.yml
```


# Clean kubernetes Cluster

```shell
ansible-playbook -i hosts master-clean.yml
```

```shell
ansible-playbook -i hosts workers-clean.yml
```

