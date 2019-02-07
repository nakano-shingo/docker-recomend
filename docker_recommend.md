---
theme : "black"
transition : "default"
slideNumber: true
---
# Dockerのススメ
株式会社テンダ　ISJシステム開発1部 <br>
中野 伸吾
---
# 自己紹介
- 名前：中野伸吾（なかのしんご）
- 2015年にテンダに新卒入社（4年目）
- Nuxt.js+Vuex / Flutterの勉強中<br>
<div style="text-align: center;">![nakano](nakano.jpg)</div>
---
# Docker<br>使ってますか？
--
# Dockerとは
- ** インフラのコード化 ** による<br>環境構築の自動化を実現するツール

- コンテナ型の仮想技術によって <br>** どこでも同じように動作する環境 ** が実現できる

- ** 軽量な動作と環境ファイル共有 ** が可能
--
# Dockerのメリット
- 環境差分を無くせる (同じ環境を簡単に再現可)

- CI/CDツールとの連携が用意<br>
※ 開発･テスト･運用のサイクルを加速できる

- `docker-compose`や`オーケストレーションツール`による **複数コンテナの管理** が便利＋手軽

--
# Dockerのデメリット
**そ ん な も の は あ り ま せ ん**
--
強いて言うならば
- 学習コスト
- OSを完全にエミュレートできない
- 使わないDockerイメージを放っておくと<br>ディスク容量を圧迫する
---
# Dockerの導入方法
--
## ①Dockerクライアントの用意

|OS|利用ツール|
|---|---|
| Windows7 | <a href="https://docs.docker.com/toolbox/toolbox_install_windows/">Docker ToolBox</a> |
| Windows10 | <a href="https://docs.docker.com/docker-for-windows/">Docker for Windows</a> |
| MacOS | <a href="https://docs.docker.com/docker-for-mac/">Docker for Mac</a> |
--
## ②Dockerfileの用意
![Dockerfile](dockerfile.png)
--
## ③Docker RUN!!!
![Docker Run](docker_run.png)
---
# Dockerを業務で<br>使ってみた感想
--
## Sさん
- dockerの設定ファイルがとにかく軽い

- docker-compseが便利。<br>簡単にRedmineサーバが立ち上げられた
--
## Kさん
- 別案件のDockerコンテナとポートの競合が発生していた

- 一台のホストPCで、複数のローカル開発環境を切り替えて使えることが便利

- まだ経験が浅い＋知見が少ないので、不慣れ
--
## その他
- Vagrantに比べると軽い

- コンテナの複数稼働により<br>本番に近いインフラ環境でテストかできる

- マウントでファイルに手軽にアクセスできる

- 誰が構築しても同じ環境ができると思ったが、ホスト側のOSの違いによって苦労した
---
# 今後について
--
## 導入実績を増やして<br>ノウハウ/ナレッジを貯める
--
## オーケストレーションツールの検証／導入を行う

<!--

テンダでは、Dockerを使って<br>Webアプリを開発しています

<a href="http://recruit.tenda.co.jp/">興味のある方は、一緒に働いてみませんか？</a>

-->

---
# おわり
ありがとうございました。