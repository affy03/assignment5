# HTTP
- HTTP  
(＝HTTPプロトコル)    
通信するときにWebブラウザとサーバーがお互いに守るお約束事。    
通信プロトコルのうちの一つ。  

- 通信プロトコル   
通信するときにお互いが守るお約束事。  
スキーム名（「https://」の部分）として指定されるのも、基本的に通信プロトコル。スマホではアプリ名をスキーム名に指定する使い方が流行っている。

  
# URL
- URL  
Webページのアドレス。Web上のリソースの場所を具体的に指定する。

> [!NOTE]
URLとURIの違い：    
URLはウェブサイトや画像ファイルの場所を特定する具体的なアドレス    
URIは書籍や学術論文を一意に特定するための識別子  

# クエリ文字列
- クエリ文字列  
キーと値のペア形式で情報を伝達するための文字列？＝。キーと値で記される。  

(例) <span>https<span>://example.com/search?q=dog         
　　https://：プロトコル  
　　example.com：ホスト名  
　　/search：パス  
　　?q=dog：クエリ文字列（qがキーで、dogが値）

> [!NOTE]
クエリとは：  
SQL言語を使ったデータベースへの命令文、もしくは、検索キーワード。キーと値で記される。
SQLとは：    
データベースとやり取りするときに使う言語。




# パス変数
- パス変数  
URI内の特定のセグメントに動的な値を埋め込むための仕組み｛｝

(例) <span>https<span>://example.com/users/{username}  
　　https：プロトコル  
　　example.com：ホスト  
　　/users/{username}：パス  
　　{username}：パス変数  
 
 「<span>https<span>://example.com/users/affy03」のように実際のユーザー名がパス変数に埋め込まれる。affy03というユーザーの情報にアクセスするためのURI。  

 

> [!NOTE]
パスとは：  
URLの一部であり、リソースがどの場所に存在するかを指定する。Windowsは（C:\Windows\system32\のように）\で、MacやLinuxは（/user/bin/pearlのように）/で区切る






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

