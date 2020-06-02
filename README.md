# Measurement application for Raspberry Pi CPU Info 
## 概要 
本プログラムはRaspberryPiのCPU情報をCSV形式で出力するプログラムである。

## 動作環境
RaspbianとPython3のインストールが必要

動作確認済みバージョン
```
python 3.7.3
```

# DEMO
```
CPU Freq(MHz), 2000, CPU Temp, 58,2'C, CPU Rate(％), 75
CPU Freq(MHz), 2000, CPU Temp, 59,2'C, CPU Rate(％), 72
CPU Freq(MHz), 2000, CPU Temp, 59,4'C, CPU Rate(％), 74
CPU Freq(MHz), 2000, CPU Temp, 58,5'C, CPU Rate(％), 78
```
 
# Usage

## 準備 
```bash
git clone https://github.com/omura0512/raspberrypi-cpu-info-measurement.git
cd raspberrypi-cpu-info-measurement
mkdir data
python cpu_watcher.py
```
## 出力値だけ見たい場合
```bash
python cpu_watcher.py
```

## 出力値を見ながらファイル出力も行いたい場合
```bash
python cpu_watcher.py | tee data/log.csv
```
 
# License
raspberrypi-cpu-info-measurement is under [MIT license](https://en.wikipedia.org/wiki/MIT_License).
