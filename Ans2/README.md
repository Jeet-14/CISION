```bash
jeet@Jeet-Desai:~/cision$ kubectl get svc,statefulset,pod,pvc
NAME                 TYPE        CLUSTER-IP   EXTERNAL-IP   PORT(S)   AGE
service/kubernetes   ClusterIP   10.96.0.1    <none>        443/TCP   17m
service/nginx        ClusterIP   None         <none>        80/TCP    4m16s


NAME                   READY   AGE
statefulset.apps/web   3/3     102s


NAME        READY   STATUS    RESTARTS   AGE
pod/web-0   1/1     Running   0          102s
pod/web-1   1/1     Running   0          82s
pod/web-2   1/1     Running   0          62s


NAME                              STATUS   VOLUME                                     CAPACITY   ACCESS MODES   STORAGECLASS   AGE
persistentvolumeclaim/www-web-0   Bound    pvc-dadfa1f1-9937-4dbb-994a-0d8a71ee469a   500Mi      RWO            standard       102s
persistentvolumeclaim/www-web-1   Bound    pvc-1170e965-6ee7-4f09-8ba4-f6fe6434eefd   500Mi      RWO            standard       82s
persistentvolumeclaim/www-web-2   Bound    pvc-0381f07c-f2ef-4ffc-a799-c36c17b7b5e8   500Mi      RWO            standard       62s
```
