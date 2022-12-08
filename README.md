# sys_prj_B01

## プログラムコンパイル
```
$ javac -d WebContent/WEB-INF/classes -cp "lib/*" src/billboard/*.java
```

## サーバーの実行
```
$ java -cp "lib/*:bin" server.AppServer 8080 /isp2 WebContent
```

## Git管理

### ファイルの修正
```
$ git add file_name
$ git commit -m "修正内容"
$ git push
```

### upstreamの設定
```
$ git remtoe add upstream 本家リポジトリURL
```

### 修正項目の申請
```
プルリクエストの作成
```

### 本家レポジトリとの同期
```
$ git fetch upstream
$ git merge upstream/master
```

### データベースの確認
```
// データベースに接続
$ sqlite3 sys_proj_B01.sqlite3

// データ表示する際にカラムを表示
sqlite> .headers ON

// テーブルの確認
sqlite> .tables

// データの確認
sqlite> select * from Ranking;
```
