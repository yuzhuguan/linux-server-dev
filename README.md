# npm配置
1. npm config ls 查看npm 配置
2. npm config set registry https://registry.npm.taobao.org  持久安装淘宝镜像包

# Linux
1. **查看物理CPU个数、核数、逻辑CPU个数**
   ```
   总核数 = 物理CPU个数 X 每颗物理CPU的核数 
   总逻辑CPU数 = 物理CPU个数 X 每颗物理CPU的核数 X 超线程数

   查看物理CPU个数
   cat /proc/cpuinfo| grep "physical id"| sort| uniq| wc -l

   查看每个物理CPU中core的个数(即核数)
   cat /proc/cpuinfo| grep "cpu cores"| uniq

   查看逻辑CPU的个数
   cat /proc/cpuinfo| grep "processor"| wc -l

   查看CPU信息（型号）
   cat /proc/cpuinfo | grep name | cut -f2 -d: | uniq -c

   查看内 存信息
   cat /proc/meminfo
   ```
