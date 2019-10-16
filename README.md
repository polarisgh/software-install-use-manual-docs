## 系统环境
**说明**：***本工程所有文档请参考规范：《文档编写格式规范-01-20190929-001.docx》***
| 项目     | 说明                                                         |
| -------- | ------------------------------------------------------------ |
| 操作系统 | ubuntu-16.04.2_x64                                           |
| 虚拟机   | VirtualBox-5.1.18                                            |
| IP       | LTSR001-192.168.0.101（单机）、LTSR002-192.168.0.102、LTSR003-192.168.0.103 |
| 超级用户 | root/smartai                                                 |
| 操作用户 | smartai/smartai                                              |

## 操作指引
```shell
# 准备
ssh-keygen -t rsa -C "youremail@example.com"
# 配置GitHub ==> Settings ==> SSH and GPG keys（~/.ssh/id_rsa.pub）
# 拉取远程仓库
cd local repositories path
# 关联远程仓库
git init
# git配置
git config --global user.name "yourname"
git config --global user.email "youremail@example.com"
# windows环境下换行问题
git config --global core.autocrlf false
# 关联远程仓库
git remote add origin git@github.com:polarisgh/software-install-use-manual-docs.git
git pull origin author
# 所有编辑工作请在author分支完成
git checkout author
# 拉取更新（提交命令前一定注意要先pull，如有冲突解决完冲突再提交）
git pull origin author
# 新增/更新
git add .
git commit -m "add/update xxx"	
git pull origin author
git push -u origin author
# 删除
git rm xxx.xxx
git commit -m "delete xxx"	
git pull origin author
git push -u origin author
```

## 版本

**说明**：***更新该列表时请按照软件名称的字典顺序编辑***


| 软件              | 版本                                                  | 来源                                                         |
| ----------------- | ----------------------------------------------------- | ------------------------------------------------------------ |
| ELK-elasticsearch | elasticsearch-6.3.0.tar.gz                            | https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-6.3.0.tar.gz |
| ELK-logstash      | logstash-6.3.0.tar.gz                                 | https://artifacts.elastic.co/downloads/logstash/logstash-6.3.0.tar.gz |
| ELK-kibana        | kibana-6.3.0-linux-x86_64.tar.gz                      | https://artifacts.elastic.co/downloads/kibana/kibana-6.3.0-linux-x86_64.tar.gz |
| Flink             | flink-1.9.0-src.tgz                                   | http://archive.apache.org/dist/flink/flink-1.9.0/            |
| Hadoop            | hadoop-2.6.4.tar.gz                                   | https://archive.apache.org/dist/                             |
| Hive              | apache-hive-1.2.1-bin.tar.gz                          | https://archive.apache.org/dist/                             |
| JDK               | jdk-8u211-linux-x64.tar.gz                            | https://www.oracle.com/technetwork/java/javase/downloads/java-archive-javase8u211-later-5573849.html |
| git-msysGit       | Git-2.17.0-64-bit.exe                                 | https://git-scm.com/download                                 |
| git-EGit          | Eclipse Marketplace                                   | https://www.eclipse.org/egit/download/                       |
| Kafka             | kafka_2.11-0.11.0.3.tgz                               | http://kafka.apache.org/downloads.html                       |
| Maven             | apache-maven-3.2.5-bin.tar.gz                         | https://archive.apache.org/dist/maven/maven-3/               |
| MySQL             | mysql-server_5.7.22-1ubuntu16.04_amd64.deb-bundle.tar | https://downloads.mysql.com/archives/community/              |
| OS                | ubuntu-16.04.2-desktop-amd64.iso                      | http://releases.ubuntu.com/16.04/ubuntu-16.04-desktop-amd64.iso |
| VirtualBox        | VirtualBox-5.1.18-114002.exe                          | http://download.virtualbox.org/virtualbox/                   |
| Zookeeper         | zookeeper-3.4.10.tar.gz                               | http://archive.apache.org/dist/zookeeper/zookeeper-3.4.10/   |

## 完成列表

**状态说明**： U-修改中；D-已完成； S-最终版；（***更新该列表时请按照软件名称的字典顺序编辑***）

| 软件  | 文件名                                                       | 环境      | 状态 |
| ----- | ------------------------------------------------------------ | --------- | ---- |
| Flink | /Flink/[安装文档]-VirtualBox_Ubuntu-16.04_Flink-cluster-06-20191009-001.docx | 离线      | S    |
| git   | /git/Git、GitHub、GitLab基本原理、安装与应用-01-20191011-001.docx | 联网/离线 | U    |
| JDK   | /JDK/[安装文档]-jdk-8u211安装文档-01-20191015-001.docx       | 离线      | S    |

