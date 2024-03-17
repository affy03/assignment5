# HTTP
### ◎HTTPとは  
- ＝HTTPプロトコル    
- 通信するときにWebブラウザとサーバーがお互いに守るお約束事。    
- 通信プロトコルのうちの一つ。  

〇通信プロトコルとは   
- 通信するときにお互いが守るお約束事。  
- スキーム名（「https://」の部分）として指定されるのも、基本的に通信プロトコル。スマホではアプリ名をスキーム名に指定する使い方が流行っている。

〇HTTPSとの違い
- httpsはhttpと暗号化と検証を加えたもの。ブラウザとサーバー間のやり取りも暗号化されているためhttpより安全。

# URL
### ◎ URLとは  
- Webページのアドレス。Web上のリソースの場所を具体的に指定する。

> [!NOTE]
> 〇URL・URN・URIの違い        
> - URL(Uniform Resource Locator)：インターネット上に存在するファイルの場所を示すもので、Web上の住所にあたる。
> - URN(Uniform Resource Name)：Web上のファイルの名前を示すもの。 
> - URI(Uniform Resource Identifier)：インターネット上に存在するあらゆるファイルを識別する総称。URL、URNはともにURIの一部。  

# クエリ文字列
### ◎クエリ文字列とは  
- キーと値のペア形式で情報を伝達するための文字列？＝。キーと値で記される。  

　(例) <span>https<span>://example.com/search?q=dog         
　　https://：プロトコル  
　　example.com：ホスト名  
　　/search：パス  
　　?q=dog：クエリ文字列（qがキーで、dogが値）

> [!NOTE]
> 〇クエリとは
> - SQL言語を使ったデータベースへの命令文、もしくは、検索キーワード。キーと値で記される。
>    
> 〇SQLとは  
> - データベースとやり取りするときに使う言語。




# パス変数
### ◎パス変数とは  
- URL内の特定のセグメントに動的な値を埋め込むための仕組み。

　(例) <span>https<span>://example.com/users/{username}  
　　https：プロトコル  
　　example.com：ホスト  
　　/users/{username}：パス  
　　{username}：パス変数  
 
 - 「<span>https<span>://example.com/users/affy03」のように実際のユーザー名がパス変数に埋め込まれる。affy03というユーザーの情報にアクセスするためのURL。  

 

> [!NOTE]
> 〇パスとは
> - URLの一部。リソースがどの場所に存在するかを指定する。Windowsは（C:\Windows\system32\のように）\で、MacやLinuxは（/user/bin/pearlのように）/で区切る。


# クエリ文字列とパス変数の違い

### ◎見た目の違い  
（例）<span>https<span>://zenn.dev/search?q=Laravel  
　　クエリ文字列：?q=Laravel   
（例）<span>https<span>://example.com/users/{username}    
　　パス変数：{username}    


### ◎中身の違い  
- パス変数：URL内の特定のセグメントに動的な値を埋め込むための仕組み 
- クエリ文字列：キーと値のペアで情報を伝達するための仕組み


### ◎目的の違い  
- パス変数：特定のリソースに対してリクエストを送る  
- クエリ文字列：リソースのフィルタリングや検索などをする  


# HTTPメソッド
### ◎ HTTPメソッドとは  
- WebブラウザからWebサーバーに対して出されるお願いの種類。

- GET  
「ページちょうだい」  

- POST  
「データどうぞ」  

- PATCH  
「データの一部を変えて」  

- DELETE  
「このデータ消して」  

# リクエストヘッダ  
### ◎リクエストヘッダとは
- リクエストを構成する部品の一つ。
- お願いに関するあれこれが書かれている場所。
- 【フィールド名】：【内容】の書式で書かれている。

> [!NOTE]
> 〇リクエストとは
>  - WebブラウザからWebサーバーに対して出されるお願い。HTTPリクエストにはPOST、GET、PATCH、DELETEを含む様々なメソッドがある。
>     
> 〇リクエストの構成要素  
> 1. リクエストライン
> 2. リクエストヘッダ  
> 　（空行）
> 3. メッセージボディ  
> 
> ◎リクエストラインとは  
> - 【どうしたい】【何を】【どんなルールで】がざっくり書かれている場所。  
>   
> ◎メッセージボディとは  
> - 補足のメモ書きが書いてある場所。  
> - POSTの場合は、受け渡されるパラメーターの内容が。GET通信のように補足の必要がない場合は何も書かれていない。



# HTTPステータスコード
### ◎HTTPステータスコードとは
- HTTPレスポンスの結果を表す３桁の数字。

- 200
「OK！ファイル送るね！」

- 201
「OK！新しいリソースを作成したよ！」(POSTに対して)

- 400
「ごめん。そのリクエスト理解でいないわ。」

- 404
「ごめん。そのファイルは持ってないわ。」

- 500
「ごめん。（サーバー側が）何かおかしい。処理方法も分からんわ。」


# レスポンスヘッダ
### ◎レスポンスヘッダとは
- レスポンスを構成する部品の一つ。
- ステータスラインで書ききれないレスポンスの情報が書かれている場所。
- 【フィールド名】【内容】で書かれている。

# レスポンスボディ
### ◎レスポンスボディとは
- レスポンスを構成する部品の一つ。
- ファイルの中身(＝HTMLファイル)が入っている。

> [!NOTE]
> 〇HTTPレスポンスとは
> - WebサーバーからWebブラウザに対して出される返事。  
>   
> 〇レスポンスの構成要素  
>1. ステータストライン  
>2. レスポンスヘッダ    
>　　（空行）  
>3. レスポンスボディ
>
> ◎ステータスラインとは  
>- レスポンスを構成する部品の一つ。
>- リクエストの結果がざっくり書かれている。
>- 【HTTPのバージョン】【ステータスコード】【ステータスコードの説明】で書かれている。

# JSON
### ◎JSONとは
- ファイルの書き方ルールの一つ。
- (例)HTML（ホームページ用）、XML、 JSON（データのやり取り用）

〇JSONを使ったデータ表現

- ピラティススタジオのクライアント情報
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

