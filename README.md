To build from git:

```
./autogen.sh && ./configure && make
```

static build:
'''
--enable-static --disable-shared LDFLAGS=-static
'''

参数意义：
‘’‘
./configure --enable-static：生成静态链接库

./configure --enable-shared：生成动态链接库

./configure LDFLAGS=-static 把static参数传入Makefile中
’‘’

注：如果 LDFLAGS=-static不生效的话，可以直接在生成的Makefile中手动修改 LDFLAGS=-static
