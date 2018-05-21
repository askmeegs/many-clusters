```
docker run \
--net=host \
-d \
-v /var/run/docker.sock:/var/run/docker.sock \
gcr.io/google_containers/hyperkube:v1.10.1 \
/hyperkube kubelet --v=2 --address=0.0.0.0 --enable_server --hostname_override=127.0.0.1 --config=/etc/kubernetes/manifests
```
