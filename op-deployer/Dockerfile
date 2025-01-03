FROM debian:bookworm-20240812-slim

# Install dependencies
RUN apt-get update && \
    apt-get install -y ca-certificates && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
    
WORKDIR /usr/local/bin

COPY op-deployer/bin/op-deployer /usr/local/bin/op-deployer

RUN chmod +x /usr/local/bin/op-deployer

CMD ["op-deployer", "--help"]
