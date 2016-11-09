# ansibleSwagger

適当なvagrantを用意して、ssh接続できるようにしておく

```
vagrant ssh-config --host 192.168.33.99 >> ~/.ssh/config
```

ansible-galaxyでロールをダウンロード(-pでディレクトリ指定。指定しないと/etc/ansibleにダウンロード)

``` 
sudo ansible-galaxy install softasap.sa-swagger-ui -p .
``` 

main.ymlとhostsを作成


```
ansible-playbook -i hosts main.yml
```

/var/www/swaggerにプロジェクトファイル群ができる(index.html)がある

/var/www/swaggerにアクセスできるようにnginxを設定して  
192.168.33.99  
にアクセスするとトップページが表示  


ansible実行先でいろいろインスコしないとansible実行時にエラーになった(なにが必要だったかわからない)

```
sudo apt-get install npm 
sudo npm install -g gulp
とか？
```
