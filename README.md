# git clone
> git clone https://github.com/tomo-gh-intro/intro.git

# 改行コードのエラー対応
エラーコード
> CRLF would be replaced by LF in @@@

gitが改行コードを変換する際に出るワーニング
以下のコマンドでgitの設定確認できる

> git config -–list | grep -i autocrlf

実行結果

> core.autocrlf=true<br>
core.autocrlf=input

trueとかinputになっていると自動変換が有効になっているらしい
以下のコマンドで設定をoffにする
> git config –-global core.autocrlf false

実行結果
> core.autocrlf=true<br>
core.autocrlf=false

