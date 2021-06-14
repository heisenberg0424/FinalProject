FROM multiarch/debian-debootstrap:mips-buster-slim as qemu

FROM scratch
ADD ./1.tar.gz /
COPY --from=qemu /usr/bin/qemu-mips-static /usr/bin
CMD ["/usr/bin/qemu-mips-static", "bin/busybox"]
ENV ARCH=mips
