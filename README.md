# Create Kubernetes Cluster


## Step 1

```
ansible-playbook -i hosts initial.yml
```
## Step 2

```
ansible-playbook -i hosts kube-dependencies.yml

```

## Step 3

```
ansible-playbook -i hosts master.yml
```

## Step 4

```
ansible-playbook -i hosts workers.yml
```



# Reset kubernetes Cluster


```
ansible-playbook -i hosts reset.yml
```


# Clean kubernetes Cluster

```
ansible-playbook -i hosts master-clean.yml
```

```
ansible-playbook -i hosts workers-clean.yml
```

