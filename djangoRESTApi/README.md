
## django REST Framework

[Qiitaの記事](https://qiita.com/kimihiro_n/items/86e0a9e619720e57ecd8#api動作確認)をベースにdjangoのREST APIのフレームワークを実装．

![rest画面](./docs/apiroot.png)

## Admin
User: rest  
pass: djangorest

## 内容
チュートリアル等で実装できるブログシステムの記事タイトル・記事内容をAPIでjson形式で取得できる．

http://localhost:8000/api/users でユーザ情報API

![](./docs/userapi.png)

http://localhost:8000/api/entries で投稿情報API  

![](./docs/entryapi.png)

### GETパラメータ
`/api/entries/?author=`で作成ユーザの絞り込みが可能．  
`/api/entries/?status=`で投稿状態を絞り込み [`public`, `draft`]
