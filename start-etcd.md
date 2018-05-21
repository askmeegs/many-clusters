```
docker run \
--net=host \
-d quay.io/coreos/etcd:latest \
/usr/local/bin/etcd --advertise-client-urls http://0.0.0.0:2379 \
--listen-client-urls http://0.0.0.0:2379 --data-dir=/var/etcd/data
```

```
docker run --net=host  -d  gcr.io/google_containers/etcd:2.0.9  /usr/local/bin/etcd --addr=127.0.0.1:4001 --bind-addr=0.0.0.0:4001 --data-dir=/var/etcd/data
```
