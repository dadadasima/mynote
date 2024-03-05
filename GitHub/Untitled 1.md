### 初始化本地仓库：

```bash
$git init
```

![image-20240305142244799](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20240305142244799.png)

### 创建秘钥：

1. 创建一个.ssh文件，可以在命令行工具中输入：

   ```bash
   mkdir .ssh
   ```

   

2. 输入

   ```bash
   $ssh-keygen -t rsa -C "GitHub邮箱号"
   ```

   生产一个RSA密钥对，`-t rsa`这个选项告诉`ssh-keygen`使用RSA算法生产密钥对；执行这个命令后，`ssh-keygen` 将在您的主目录下的 `.ssh` 文件夹中生成一个新的RSA密钥对，通常是 `id_rsa`（私钥）和 `id_rsa.pub`（公钥）。私钥用于身份验证，而公钥用于在其他系统上验证您的身份。生成的密钥对可以用于SSH连接以及其他安全通信需求。

![image-20240305142854961](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20240305142854961.png)

### 将公钥粘贴到GitHub上：

### 建立本地仓库与远程仓库连接：

```bash
git remote add origin http://... #项目地址
```

