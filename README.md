huangying, email: hy_gzr@163.com <br>
### 本项目用于交流和学习，请勿用于非正当途径

基于xdp_packet开发的高性能TCP协议的syn报文发送工具<br>
### 获取:
git clone https://github.com/huangying1980/xdp-synflood.git
### 依赖:
xdp_packet: https://github.com/huangying1980/xdp_packet.git
xdp_packet的依赖请参考xdp_packet中的README.md
### 使用:
./synflood --help
### 编译
1.  获取xpd_packet: git clone https://github.com/huangying1980/xdp_packet.git
2.  编译xdp_packet,请参考xdp_packet中的README.md，得到libxdppacket.a和xdp_kern_prog.o
3.  git clone https://github.com/huangying1980/xdp-synflood.git
4.  cd xdp-synflood
5.  复制xdp_packet/xdp_kern_prog/xdp_kern_prog.o到xdp-synflood目录<br>
    或ar -x libxdppacket.a xdp_kern_prog.o然后复制到xdp-synflood目录中
6.  make
