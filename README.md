# thanos-s3

Thanos S3 remote write and read.

## OpenShift

Setup `minio`, `thanos` and `user-workload-monitoring` to store scraped user workload metrics into s3.

```bash
oc apply -k ocp/
```

## Locally

More complete example running locally.

```bash
./generate-configs.sh
podman-compose up -d
```

- http://localhost:10904/graph
- http://localhost:9001/buckets/thanos/browse
- http://localhost:3000/login

## Links

- https://docs.openshift.com/container-platform/4.10/monitoring/configuring-the-monitoring-stack.html#configuring_remote_write_storage_configuring-the-monitoring-stack
- https://blog.ruanbekker.com/blog/2020/02/01/setup-thanos-on-docker-a-highly-available-prometheus
- https://aws.amazon.com/blogs/opensource/improving-ha-and-long-term-storage-for-prometheus-using-thanos-on-eks-with-s3/
- https://github.com/thanos-io/thanos/blob/main/docs/components/sidecar.md
- https://thanos.io/tip/components/receive.md/