# Update Deployments

1. First approach (recommended):
```sh
kubectl set image deployment <deploy-name> <container-name>=<image-name>:<image-version>
kubectl annotate deployment <deploy-name> kubernetes.io/change-cause="<update text>"
```

2. Second approach:
```sh
kubectl edit deployment <deploy-name>

- change the version of the image
- change the annotation "kubernetes.io/change-cause" of the deployment

```

3. Third apprach (depracated):
```sh
kubectl set image deployment <deploy-name> <container-name>=<image-name>:<image-version> --record
```
