# thanos-s3

Thanos S3 remote write and read

https://blog.ruanbekker.com/blog/2020/02/01/setup-thanos-on-docker-a-highly-available-prometheus
https://aws.amazon.com/blogs/opensource/improving-ha-and-long-term-storage-for-prometheus-using-thanos-on-eks-with-s3/
https://github.com/thanos-io/thanos/blob/main/docs/components/sidecar.md

```bash
./generate-configs.sh

podman-compose up -d
```

http://localhost:10904/graph

http://localhost:9001/buckets/thanos/browse

http://localhost:3000/login