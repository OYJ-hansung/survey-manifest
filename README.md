# Eureka-manifest

# How To Use
1. change the base file(.yaml) in the base directory and modify the kustomize file to apply the change
2. go to the /overlays/dev/ folder and update the tag using the following command

```shell
kustomize edit set image ghcr.io/wlgns5376/example-app:latest
```
3. apply the following command to apply and build your new image to the repository

```shell
kustomize build .
kubectl apply -f -
```

4. git push the new file
