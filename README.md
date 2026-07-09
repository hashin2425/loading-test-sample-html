# loading-test-sample-html

読み込みテスト用の HTML ファイル（GitHub Pages）

```sh
ls docs/ -l
```

- <https://hashin.net/loading-test-sample-html/size-10b.html>
- <https://hashin.net/loading-test-sample-html/size-1kb.html>
- <https://hashin.net/loading-test-sample-html/size-1mb.html>
- <https://hashin.net/loading-test-sample-html/sample.html>
- <https://hashin.net/loading-test-sample-html/connectivity-check.html>

## URL Connectivity Check

<https://hashin.net/loading-test-sample-html/connectivity-check.html>

スマホ向けの疎通確認ページです。

- README に記載している URL を順番に fetch して疎通確認
- 初期状態では `size-10b.html` のみ有効
- URL ごとにオン/オフを切り替え可能
- 確認間隔は `0.2秒` / `1秒` / `5秒` / `10秒` / `60秒` から選択可能
- fetch のタイムアウトは 3 秒。タイムアウトはエラーとして集計
- 上部に確認回数、成功数、エラー数、累積通信量を表示
- 最終疎通時刻、通信時間、推定通信速度を URL ごとに表示
- 直近 10 分の成功/エラー履歴をグラフ表示
- アナリティクス情報は localStorage に保存し、リロード後も維持
