# FixQb_Back_Reload
qbittorrent备份迁移降级跳检

### 傻瓜教程——Linux版本，首先qbittorrent开启webui. SSH登入机器。以xshell连接Ubuntu系统为例：

#### 下载：

演示过程——进入家目录创建一个my_code文件夹，进入文件夹后克隆本GitHub项目到本地。进入目录后观察是否已经下载。主要代码如下：

`git clone https://github.com/tomorrow505/FixQb_Back_Reload.git` 

![演示](https://s2.ax1x.com/2020/03/07/3XwjH0.png)

#### 拷贝种子文件：

首先找到qbittorrent备份种子目录，然后创建一个torrent目录，将其中所有文件拷贝到torrent文件夹中，主要代码如下：

```
find / -name BT_back*  找到qbittorrent备份种子的目录
mkdir torrent          在当前文件夹下创建一个torrent目录
cp ***/BT_backup/* ./torrent  将步骤1输出的目录中的文件拷贝到torrent目录下

#下边两步是为了让大家看清楚操作过程
cd torrent                  进入torrent目录  
ls					      列出目录中的文件

cd ..                       返回上一级目录
```

![拷贝种子](https://s2.ax1x.com/2020/03/07/3XBKoV.png)

![操作界面](https://s2.ax1x.com/2020/03/07/3jk9BV.png)
