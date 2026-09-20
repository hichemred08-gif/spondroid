FROM alpine:3.18

RUN apk add --no-cache \
    bash \
    git \
    openssh \
    openrc \
    sudo \
    curl \
    nano \
    vim \
    qemu \
    qemu-img \
    qemu-system-x86_64

RUN ssh-keygen -A

EXPOSE 22

CMD ["/usr/sbin/sshd", "-D"]
