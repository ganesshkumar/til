---
description: Syncing docker container clock
---

# Syncing Container Clock

By default docker container’s will sync their time with the local system time but the default timezone is “UTC”. If you are using `Date` or `Time` in your application, you have to manually set the timezone for the container. One easy way to do so is using the environmental variable `-e "TZ=Asia/Kolkata"`.

But sometimes, the container time will deviate a little from the local system time. OS X, linux and unix have `/etc/localtime` file by default. You can mount this file as a read-only file inside the container to sync the container's time `-v /etc/localtime:/etc/localtime:ro`.
