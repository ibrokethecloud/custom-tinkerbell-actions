# reboot action

Needs following action definition

```
          - name: "reboot"
            image: gmehta3/reboot:latest
            timeout: 90
            volumes:
            - /worker:/worker
```