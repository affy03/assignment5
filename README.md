# HTTP
### HTTPとは
通信プロトコルのうちの一つ。  
通信プロトコルは通信するときにお互いが守るお約束事。  
スキーム名（「https://」の部分）として指定されるのも、基本的に通信プロトコル。スマホではアプリ名をスキーム名に指定する使い方が流行っている。


### HTTPプロトコルとは
通信するときにWebブラウザとサーバーがお互いに守るお約束事。  

  
# URL
### URLとは
Webページのアドレス。Web上のリソースの場所を具体的に指定する。

> [!NOTE]
URLとURIの違い：    
URLはウェブサイトや画像ファイルの場所を特定する具体的なアドレス    
URIは書籍や学術論文を一意に特定するための識別子  

# クエリ文字列


# パス変数

# HTTPメソッド

# リクエストヘッダー

# HTTPステータスコード

# HTTPレスポンスヘッダー

# HTTPレスポンスボディ


# JSON
### JSONを使ったデータ表現

ピラティススタジオのクライアント情報
```Json
{
    "company":"Pilates Studio A"
    "clients":[
        {
            "id":1,
            "name":"will smith",
            "age":55,
            "condition":"lordosis"
            "plan":"4 times a month"
        },
        {
           "id":2,
            "name":"Natalie Portman",
            "age":42,
            "condition":"thoratic scoliosis"
            "plan":"2 times a week" 
        },
        {
            "id":3,
            "name":"Jennifer Lawrence",
            "age":33,
            "condition":"flat back"
            "plan":"4 times a month"
        }
    ]
}
```

