# fastdfs

## 1、启动tracker方式
```
docker run -e SERVER=tracker -v [/root/fdfs]:/etc/fdfs [-v /fastdfs/tracker:/fastdfs/tracker] \
 [-p 22122:22122] --name tracker -d yuyiyu/fastdfs:2.0
```

## 2、启动storage方式
```
docker run -v [/root/fdfs]:/etc/fdfs [-v /fastdfs/storage:/fastdfs/storage] \
 [-p 23000:23000 -p 8888:8888] --name storage -d yuyiyu/fastdfs:2.0
```

## 3、说明
> storage中的tracker配置需按情况变更
