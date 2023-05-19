# ジーズクエスト［リッチ版］
## https://github.com/T49Miuratch/GS_QUEST2_RICH

  - デプロイしている場合はURLを記入（任意）

## 紹介と使い方
「じゃんけん」をドラクエ風のゲームにしたいと思い改造しました。
せっかく作ったのでデプロイして、Stable Diffusionで生成した美女キャラクターと野球拳するゲームに切り替えてアフィを稼げたらと考えております。

# 工夫した点
複数の関数を一つのjsにまとめて作っていたのですがどうももうまくいかず、どこのなにがエラーなのか、なぜ動かないのか、わからなくなってしまい途方にくれました。
仕方ないので、以下のような関数をひとつずつテスト用のjsとして個別に作成し、動作確認を行い、最終的にそれを取りまとめる形で実装しました。
なのでテスト用のhtmlには山ほどjsを紐づけました。

<ul>
<li>ボタンを押すとランダムで数字（ヒットポイント）が減る
<li>数字が0になると特別なメッセージ（プレイヤーはたおれた！　or モンスターをやっつけた！）が出る
<li>上記の「プレイヤーはたおれた！」メッセージ後に画面が暗くなり、「リプレイ？」ボタンが出る
<li>上記の「モンスターをやっつけた！」メッセージ後に画面が明るくなり、「congratulation! もういちどあそぶ？」ボタンが出る
<li>URLを開くとモーダルウインドウが開く。ボタンを押すと音楽が流れる
<ul>
  
# 苦戦した点
<ul>
<li>class（.）とid（#）を混同して動かないことに四苦八苦しました
<li>ChatGPTに頼ったのですがあまり思い通りにコードを書いてくれず、BingAI（GPT4）に任せたらかなり精度が高まりました
<li>が、Bingのもそのままでは動かず、console.logで動作確認をしても動かず、悩んだ結果、吐き出させたhtmlの<script>タグがhead内に書かれていたのが原因でした
<li>元々（前回提出）のjsコードをいじっていたらいろいろいじりすぎて修復不能になり、gitから戻して再構築等を行いました
</ul>  
  - 明日の自分への伝言

  ・夜は眠くて作業が非効率なので、早朝起きでがんばろう
  
## 参考にした web サイトなど

bing AI
