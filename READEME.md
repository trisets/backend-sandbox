### コンテナの起動方法
1. BACKEND-SANDBOXのディレクトリに移動する
1. docker image を作成する
    + docker image build -t keycloak:v1 .
1. イメージからコンテナを立ち上げる
    + docker run -e KEYCLOAK_USER=admin -e KEYCLOAK_PASSWORD=admin -dp 8080:8080 --name keycloak-container -it keycloak:v1
    
1. コンソール画面にアクセスする
    + http://localhost:8080/auth/
        + レスポンスがあるまで数分かかる場合がある

2. アドミンコンソールにログインし、色々できる


<br>

[参考サイト](https://thinkit.co.jp/article/17621)