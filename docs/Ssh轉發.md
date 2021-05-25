https://beginor.github.io/2020/05/13/sumary-of-port-forward-with-ssh.html


# 本地轉發/正向代理(-L)
在本地啟動端口，把本地端口數據轉發到遠端。
ssh -N -L localhost:8000:iqm.ddns.net:8000 us@iqm.ddns.net

# 動態代理/socks5代理(-D)
SwitchyOmega 在鍵入socks5://127.0.0.1:8888代理
ssh -C -T -N -D 127.0.0.1:8888 us@iqm.ddns.net
curl -i --proxy socks5://127.0.0.1:8888 ifconfig.me

# 遠端代理/反向代理(-R)
ssh -T -N -R iqm.ddns.net:8088:localhost:5000 us@iqm.ddns.net


-C為壓縮數據
-q安靜模式
-T禁止遠程分配終端
-n關閉標準輸入
-N不執行遠程命令
此外視需要還可以增加-f參數，把ssh放到後台運行。