# EnvTest
To test environment about mongodb and mysql in the docker and test to connect with pymongodb and pymysql.

# 基礎環境建置

## 環境前提
 * docker & docker-compose in linux with VMWare
 * jupyter notebook with python in windows
## docker-compose.yml
  * 在linux下: <br>
    1.請先建置一個資料夾，我自己是建一個叫env的資料夾，以下將以env資料夾作為範例。 <br>
    2.將docker-compose.yml放在env資料夾下。 <br>
    3.在terminal中輸入`docker-compose up -d` 。 <br>
      ![image](https://user-images.githubusercontent.com/53245830/120437306-82252700-c3b2-11eb-985e-41221f602aed.png) <br>
    4.可以在terminal輸入`docker ps` 確認container有無建起。
      ![image](https://user-images.githubusercontent.com/53245830/120437522-bef11e00-c3b2-11eb-90d2-0eceb72e9b2f.png)
  
## DB連線測試_Git.ipynb
  * 在windows下: <br>
    1.打開jupyter notebook以便打開此檔。<br>
    2.尚未安裝pymysql以及pymongodb者，請依序安裝。<br>
    3.請先在linux中的terminal輸入`ifconfig`找到ens32，inet就是你的ip位址，像我的是192.168.XXX.XXX。
      ![image](https://user-images.githubusercontent.com/53245830/120438435-f1e7e180-c3b3-11eb-85b8-63c99923ea0e.png)

    4.請在DB連線測試_Git.ipynb中需要輸入ip的地方輸入你剛剛在linux下找到的ip。
      ![image](https://user-images.githubusercontent.com/53245830/120439466-20b28780-c3b5-11eb-8648-d6e6a9014cca.png)
      ![image](https://user-images.githubusercontent.com/53245830/120438867-70448380-c3b4-11eb-877e-566dba090b5e.png)
    5.接著依序測試程式，如果跟以下畫面結果相同及成功。
      ![image](https://user-images.githubusercontent.com/53245830/120439784-8272f180-c3b5-11eb-9567-512c77884089.png)
      ![image](https://user-images.githubusercontent.com/53245830/120439852-93bbfe00-c3b5-11eb-878a-17c826ee561a.png)
