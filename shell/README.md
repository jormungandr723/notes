# Shell

## 在Ubuntu里面的坑

```shell
root@iZm5ebwtdyoe99lpvnt1o6Z:~# ll /bin/sh
lrwxrwxrwx 1 root root 4 Dec 14 18:54 /bin/sh -> dash*
```

默认为dash，而不是bash

解决办法:

1. 使用bash执行
2. 脚本里面添加#!/bin/bash,然后添加执行权限，使用.执行
3. 修改软连接,指向bash