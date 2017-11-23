---
description: Remove all dangling volumes
---

# Remove all dangling volumes

While using data volume containers, you have to remove container with -v flag as docker rm -v. If you don't use the -v flag, the volume will end up as a dangling volume and remain in to the local disk

To delete all dangling volumes, use the following command

```
docker volume rm `docker volume ls -q -f dangling=true`
```
