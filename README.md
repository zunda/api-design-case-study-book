# 「APIデザインケーススタディ ――Rubyの実例から学ぶ。問題に即したデザインと普遍の考え方」サポートページ

- 書名: APIデザインケーススタディ ――Rubyの実例から学ぶ。問題に即したデザインと普遍の考え方
- 著者: 田中 哲
- ISBN: 978-4-7741-7802-8
- 奥付発行日：2016年1月25日
- 店頭発売日：2015年12月16日
- シリーズ: WEB+DB PRESS plusシリーズ
- 出版社: 技術評論社
- 技術評論社の書籍案内: http://gihyo.jp/book/2016/978-4-7741-7802-8
- サポートページ: https://github.com/akr/api-design-case-study-book

## 正誤表

### 間違い:

- p.89 Socket クラスの勧め
  「また、recv_io, recv_io メソッドは後述する recvmsg, sendmsg メソッドで対応します。」->
  「また、recv_io, send_io メソッドは後述する recvmsg, sendmsg メソッドで対応します。」

- p.236 秒未満の表現
  「`2**-64`秒 (約`54.2**-21`秒)」 ->
  「`2**-64`秒 (約`54.2*10**-21`秒)」

### 間違いに見えるが間違いではない:

- p.92 Socket.ip_address_list
  「実際、名前解決では 127.0.1.1 だけが返ってくるなど、期待されない結果になることもよくあります。」
  127.0.1.1 は間違いと感じられるかもしれませんが、
  Debian GNU/Linux はいつのころからか /etc/hosts で、
  localhost は 127.0.0.1, ユーザが決めたホスト名は 127.0.1.1 を返すように設定されるようになりました。
  このことについては Debian のマニュアルの
  https://www.debian.org/doc/manuals/debian-reference/ch05.en.html#_the_hostname_resolution
  というところに書いてあります。

