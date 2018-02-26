# ライフゲームを作ってみた話

---

### なぜライフゲームなのか

言語を学んだ後になにを作るかで悩むことが多かった


---

### こんな記事を発見

![HelloWorldのあと](./img/afterhelloworld.png)

http://razokulover.hateblo.jp/entry/2017/05/23/131359

---

### ブコメにこんなコメントが

![mizchiさんのブコメ](./img/mizchi.png)

---

# なるほど🤔

---

### ライフゲーム

* 「Conway's Game of Life」と呼ばれている
* 生命の誕生、進化、淘汰を簡単なモデルで再現したシミュレーションゲーム
* 単純なルールで状態の変異を試すことができる

![こんな感じのヤツ]()

---

状態の変更が激しいため、状態管理を簡単にするフレームワークである **React** を試すのに良さそうなお題

---

### ライフゲームのルール

* 誕生
  * 死んでいるセルに隣接する
* 生存
  *
* 過疎
  * 
* 過密

---

# デモ

https://github.com/otakumesi/lifegame

---

### 構成
とりあえず詰め込めそうな奴を詰め込んだ

- ES6
  - preset-env
  - preset-react
  - plugin-propsal-object-rest-spread
- React
- Redux
- postcss

---

### 実際に作ってみてどうよ
正直なところ反省している。

* どう考えても今回の構成にReduxはいらなかった
  * そんな大きな状態管理をしていない...
  * モチベ的にはあまり触ってないものを触れたかったので、MobXあたりがよい落とし所だったか

---

### ボイラープレート作った
さすがに毎度package集めて、webpackの設定をアレするのはつらい。

https://github.com/otakumesi/dotfiles/tree/master/.project.template/frontend

---
