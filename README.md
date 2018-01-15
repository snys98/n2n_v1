# N2N VPN v1

### N2N VPN是一个部署和使用都比较方便的VPN, 此Repo只保证服务端supernode可以编译通过. 原repo(https://github.com/ntop/n2n) 编译成Windows的版本操作起来实在是比较麻烦, 所以这里单独建了一个repo来处理windows下面supernode的编译, 特纪录在此, 以备后用.

### 关于N2N的更多介绍和客户端的使用请参考网上的文章

## 编译:

### 前置条件: vs2017(需安装C++开发模块)

### 操作:

打开位于".\win32\DotNet"目录下的n2n.sln, 修改supernode项目的windows sdk的版本至本机版本, 生成supernode项目, 对应的supernode.exe文件位于".\win32\DotNet\Release"目录下

#### 这里提供一个本人于win10 insider下编译的supernode.exe(https://gist.github.com/snys98/2dc46951e0d9532fc997578d95a45435)

## 使用

### 前置条件: 有固定ip的云服务器, 安装有和vs对应版本的vcredist

### 操作:

cd 至supernode.exe所在文件夹
```powershell
# 端口号任意指定即可(注意配置云服务器防火墙规则)
.\supernode.exe -l <端口号>
```
