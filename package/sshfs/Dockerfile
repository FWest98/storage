FROM ubuntu:16.04
RUN apt-get update && \
    apt-get install -y sshfs
COPY storage /usr/bin
COPY sshfs/rancher-sshfs common/start.sh common/common.sh /usr/bin
CMD ["start.sh", "storage", "--driver-name", "rancher-sshfs"]