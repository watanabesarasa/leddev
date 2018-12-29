# leddev
robsys2018 課題１
Lチカ

## 概要
LEDを様々に光らせるデバイスドライバ

## 必要なもの
-  Raspberry Pi 3 Model B V1.2
  -  Raspbian
-  LED 1つ
-  Linux カーネルソース
  -  カーネルソース を /usr/src/linux　にダウンロード
  -  https://github.com/ryuichiueda/raspberry_pi_kernel_build_scripts.git

## 使用方法
```
cd leddev
make
sudo insmod myled.ko
sudo chmod 666 /dev/myled0
echo 0 > /dev/myled0 //消す
echo 1 > /dev/myled0 //光る
echo 2 > /dev/myled0 //2回点滅
echo 3 > /dev/myled0 //3回点滅
echo 4 > /dev/myled0 //4回点滅
echo 5 > /dev/myled0 //カエルの歌のリズムで光る
```
## Licence
-  GPLv3 license
-  
