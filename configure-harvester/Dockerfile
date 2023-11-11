FROM alpine
RUN apk add parted curl zstd e2fsprogs e2fsprogs-extra bash sgdisk yq
ADD configure-harvester /bin/configure-harvester
CMD [ "/bin/configure-harvester" ]
