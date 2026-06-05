# BOOLE

神奈川県大和市のヘアサロン「BOOLE」のサイト。
Three.js のアイソメ・ジオラマ＋黒板チョークループ。モバイルファースト。

- `index.html` … 単一ファイル（外部依存は Three.js の CDN のみ）
- `assets/diorama.glb` … 3Dジオラマ
- `assets/logos/` … 黒板に出るロゴ各種
- `assets/poster.jpg` … WebGL不可時のフォールバック

ローカル確認:

```
python -m http.server 8000
# → http://localhost:8000/
```

※ ES モジュール＋fetch のため `file://` では動きません（要サーバー or GitHub Pages）。
