
##配置文件恢复方法: 在设置页面定时设定里增加下面一行，保存后会自动更新：         
22 * * * * bash /root/jd/git_pull.sh >/dev/null 2>&1 
##更新时间为每小时的第22分钟 


#已经添加支持手机运行， 可以用闲置的安卓手机安装App后添加面板设置脚本运行!
# 安卓手机安装运行方法:[点击查看](https://github.com/hajiuhajiu/jdsign1112/blob/master/icon/Termux.md)



# git hub action
不要用action跑， 否则github封号，  Action 打开方式 setting--actions ......Actions permissions
.........Allow all actions...save 

# docker 一键安装：
可以下载putty，进入终端，复制下面命令，按提示操作，不知道怎样填就默认回车：

wget  https://gitee.com/xr2021/jd-shell/raw/v3/install_scripts/docker_install_jd.sh -O docker_install_jd.sh && chmod +x docker_install_jd.sh && bash docker_install_jd.sh

安装完成后输入docker设备地址如192.168.1.1:5678 用户名admin密码admin5678 添加cookie，自行设定各脚本运行时间即可。



# 扫码获取ck目前失效! 需要手动找cookie[点击查看](https://github.com/hajiuhajiu/scripts/blob/master/icon/GetJdCookie.md)  

低调使用，不要fork！尽量第一时间同步更新脚本。
防止失联请收藏gitee备份地址：https://gitee.com/xr2021/jdsign   

# 建议安装docker可视化管理工具portainer,可以管理docker容器察看状态 

docker pull portainer/portainer

docker run -d -p 9000:9000 -v /root/portainer:/data -v /var/run/docker.sock:/var/run/docker.sock --name dev-portainer portainer/portainer
