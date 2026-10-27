# crowd

セルフカフェ公式サイト（selfcafe.jp）・公式LINE から開く「店内の混雑状況（目安）」ページ。

- 店内カメラの映像から席の埋まり具合を15分ごとに判定した結果を、店ごとに5段階で表示する
- 現在地または店名・地名から、近い店の混み具合を表示する
- `index.html` は生成物。元は selfcafe-automation の `web/crowd/index.html`、生成は `py scripts/crowd_page.py`
- パラメータ: `?notitle` 見出しを隠す / `?store=店名` その店だけ / `?demo` 見本のデータで表示

埋め込み例:

```html
<iframe src="https://selfcafe.github.io/crowd/?notitle" width="100%" height="900" style="border:0" allow="geolocation" loading="lazy" title="店内の混雑状況"></iframe>
```
