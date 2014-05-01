﻿これはGitHubでドキュメントを公開するにはどうしたらいいか、というブログ記事用のデモリポジトリです。

## ドキュメントの記法

- マークダウン形式で書きます。
	- https://guides.github.com/features/mastering-markdown/
- ただ色々おぼえなくても、基本は次のようなものだけ覚えておけばとりあえずｊは十分かと
	- むしろ色々おぼえて凝るよりも、シンプルな文章を心がけたほうがいいかと思います

		<table><tr><td>
		\#大タイトル<br>
		\# 中タイトル<br>
		\#\# 小タイトル
		</td></tr></table>

		<table><tr><td>
		- 箇条書き
			- タブでインテント
				-  さらにタブでインテント
		- 箇条書き
		- 箇条書き
		</td></tr></table>

		<table><tr><td>`コード`</td></tr></table> .. 文中で利用する場合（<code>\`</code>の前後にスペースが必要）


		<table><tr><td>
		空行		
		> 引用したい文
		空行		
		</td></tr></table>

## ページを作ってリンクを張る

- 適当にファイルを `○○.md` として作成してコミット＆プッシュします。
- リンクを張りたい場合は
	- `[リンク名](○○.md)` と記載します。
	- こんな感じ → [リンクテスト](ドキュメント１.md)
- フォルダ作って階層を分けてもＯＫです。
	- `[リンク名](△△/○○.md)` と記載します。
	- こんな感じ → [リンクテスト](hogeディレクトリ/ドキュメント２.md)

## 画像を張る

- まず利用する画像もこのリポジトリにコミット＆プッシュしておきます。
	- 仮に `images` フォルダに格納するとします。
- こういう風にリンクを張ります。
	- `![alt内容（マウスカーソルが当たったときの表示テキスト）](images/○○.jpg)`
	- こんな感じ↓

		![alt内容](images/ichigo.jpg)

## ほか

- リンクや画像は `http(s)://～` で書けばリポジトリ外のものでもＯＫです。
- 絵文字も使えます。
	- 使える絵文字はこちら
		- http://www.emoji-cheat-sheet.com/
	- 例えばこういう風に書けばＯＫです。
		- `:smile:` → :smile:
- 個人的に参考になるGitHub上のドキュメント
	- [cookpadさんのコーディングガイドライン](https://github.com/cookpad/styleguide)
	- [mixiさんのトレーニング資料](https://github.com/mixi-inc/iOSTraining)
		- いろいろありますが、これはiOSのもの
		- こちらは目次だけリポジトリで管理して、各ページはそのリポジトリのWikiで管理するタイプ
