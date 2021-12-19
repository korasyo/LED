# Led lights up

必要なもの  
Raspberry Pi 3＋(セットアップ済み)  
ブレッドボード  
LED　1コ  
220Ω抵抗  

回路の写真  
![image](https://user-images.githubusercontent.com/95561892/146666376-e8fa31e7-f270-4efa-9d26-30a769610be0.png)  

利用したデバイスドライバ  
ロボットシステム学で上田先生が講義していたデバイスドライバ

ビルド方法  
git clone git@github.com:korasyo/LED.git
cd LED/myled  
make  
sudo insmod myled.ko  
sudo chmod 666 / dev/myled0

実行方法
echo 1 > /dev/myled0　LEDが点灯する  
echo 0 > /dev/myled0　LEDが消灯する  
