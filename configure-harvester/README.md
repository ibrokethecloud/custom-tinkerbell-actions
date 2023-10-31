# configure-harvester action

The action performs the following steps:
* fix partition table after image has been streamed to target
* resize LH partition to grow to use all available space on disk
* copy cloud-init if needed to /oem/userdata.yaml
* update terminal in grub kernel arguments

Needs following action definition

```
          - name: "configure-harvester"
            image: gmehta3/configure-harvester:latest
            timeout: 3000
            env:
              HARVESTER_TTY=tty1
              HARVESTER_DEVICE=/dev/vda
              HARVESTER_STREAMDISK_CLOUDINIT_URL=hegel-cloud-init-reference
```