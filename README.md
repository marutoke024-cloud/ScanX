# ScanX

別端末の画面をスクロール撮影して、文字と表を抽出するPWAです。

## 配置（GitHub Pages）
1. リポジトリを作り、このフォルダの中身をすべてルートに置く
2. Settings → Pages → Branch を `main` / `(root)` にして保存
3. 発行されたURLをスマホのChromeで開き、メニューから「ホーム画面に追加」

カメラはHTTPSでのみ動きます（GitHub PagesはHTTPSです）。

## 読み取り方式
- 端末内OCR: 通信なし・無料。初回のみ辞書（日本語・英語）をダウンロード
- 高精度（API）: 設定でAnthropic APIキーを入力。表の枠組みまで再現。APIの利用料がかかる

## ファイル
- `index.html` アプリ本体
- `sw.js` オフライン用サービスワーカー
- `manifest.webmanifest` / `icon*.png` / `icon.svg` ホーム画面用
