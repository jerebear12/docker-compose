FROM chrislusf/seaweedfs

COPY security.toml /etc/seaweedfs

RUN mkdir "/etc/seaweedfs/certs"

COPY master01.crt /etc/seaweedfs/certs
COPY master01.key /etc/seaweedfs/certs

COPY volume01.crt /etc/seaweedfs/certs
COPY volume01.key /etc/seaweedfs/certs

COPY filer01.crt /etc/seaweedfs/certs
COPY filer01.key /etc/seaweedfs/certs

CMD ["filer", "-s3"]
