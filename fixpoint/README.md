programテスト用program

使用環境
・python3.6
・windows8.1

使用ライブラリ
・import pandas as pd
・import apache_log_parser
・import collections
・from pprint import pprint

install
・$ pip3 install apache-log-parser

使用アクセスデータファイル名
・access_log1~100

・アクセスログの構成
%h = 10.2.3.4:リモートホスト名
%l = -:クライアントの識別子
%u = -:認証ユーザー名
%t = [18/Apr/2005:00:10:47 +0900]:リクエストを受信した時刻([day/month/year:hour:minute:secondzone]の書式)
"%r" = "GET / HTTP/1.1":リクエストの最初の行
%>s = 200 854:最後のレスポンスのステータス
%b = "-":HTTPヘッダを除くレスポンスのバイト数。0バイトの場合は「-」と表示される
"%{Referer}i" = "Mozilla/4.0":サーバが受信したリクエストヘッダのReferer
"%{User-Agent}i" = "(compatible; MSIE 5.5; Windows 98)":サーバが受信したリクエストヘッダのUser-Agent

(問3) 期間の指定について
期間指定する際は年,月,日にちを以下の通りに入力してください。
年:西暦で入力してください ex)2000,1999,2019
月:入力が一桁の場合、二桁目に0を入力してください　ex)01,06,09
日にち:入力が一桁の場合、二桁目に0を入力してください　ex)01,06,09
最後に、年,月,日を入力する場合、間に半角スペースを入力してください。 ex)2000 01 01,1999 06 06
