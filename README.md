# BOOLE

神奈川県大和市のヘアサロン「BOOLE」のサイト。
Three.js のアイソメ・ジオラマを入口に、エディトリアルなブランドページへつながるモバイルファーストのサイト。

- `index.html` … 3Dサロンのファーストビュー（外部依存は Three.js の CDN のみ）
- `about.html` … Concept / Works / Staff / Service / Access / Reservation をまとめたブランドページ
- `gallery/` … 実際のヘアスタイル写真
- `staff/` … スタッフ写真
- `assets/diorama.glb` … 3Dジオラマ
- `assets/floor_counter_opt.glb` … 床とカウンターのベイク済みモデル
- `assets/logos/` … 黒板に出るロゴ各種
- `assets/poster.jpg` … WebGL不可時のフォールバック

アニメーションはブラウザ標準APIのみで実装し、`prefers-reduced-motion`、キーボード操作、遅延画像読み込みへ対応しています。

ローカル確認:

```
python -m http.server 8000
# → http://localhost:8000/
```

※ ES モジュール＋fetch のため `file://` では動きません（要サーバー or GitHub Pages）。
