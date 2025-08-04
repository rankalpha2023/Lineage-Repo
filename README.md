# Lineage 20.0 .repo split block zipfile

1. 安装 aria2

sudo apt update

sudo apt install aria2

2. 下载所有分卷文件

aria2c -c -j 5 -i urls.txt

3. 解压缩所有文件

cat lineage-20.0_* | tar -xvf -

4. 同步文件

repo sync -c -j8