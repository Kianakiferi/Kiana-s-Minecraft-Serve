## Minecraft Servers Codes

- 建立一个screen
screen

- 使用 Mcsmanager 面板 
https://github.com/Suwings/MCSManager

```
/root/mcsmanager
npm start 
node -v
```

### Minecraft Overviewer
http://docs.overviewer.org/en/latest/


```
cd {filePath}/overviewer/overviewer.exe "saves\world" Maps
//        地图路径    输出路径
```

### 阿里云ECS 文件转移至 OSS
https://blog.csdn.net/weixin_36171533/article/details/83657732

服务器下载太慢了，影响服务器，改用OSS下载飞快

- 在服务器安装ossutil
```
./ossutil config -e oss.aliyuncs.com -i YourAccessKeyID -k YourAccessKeySecret
生成的配置文件在/root/.ossutilconfig
```
- 上传单个文件：
```
cd "ossutil文件所在目录"
./ossutil cp world.zip oss://kianakiferi
```

- 上传文件夹：
```
cd "ossutil文件所在目录"
./ossutil cp -r world oss://kianakiferi
```
