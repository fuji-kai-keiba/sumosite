# SUMO / SCROLL THE RING

スクロールに合わせて相撲動画を送り、競技の基本を読む静的なWebページです。HTML・CSS・JavaScriptで構成し、ビルドやパッケージのインストールは不要です。

## ローカルで見る

リポジトリを取得し、Python 3.13以降を推奨環境として、次を実行します。

```sh
git clone https://github.com/fuji-kai-keiba/sumosite.git
cd sumosite
python3 -m http.server 8000 --bind 127.0.0.1
```

ブラウザで `http://127.0.0.1:8000` を開きます。Windowsでは `python3` を `py -3` に読み替えてください。8000番が使用中の場合は別の空きポートを指定します。

- `index.html`: ページ本体。
- `assets/sumo.mp4`: 表示用動画。利用条件は[素材の注意事項](ASSET_NOTICE.md)を確認してください。
- [DESIGN_BRIEF.md](DESIGN_BRIEF.md): 設計方針。

## ライセンスと素材

コードと文書は [MIT License](LICENSE) です。**`assets/sumo.mp4`はMITの対象外です。** このリポジトリは動画の利用・再配布に関する追加の許諾を与えません。公開・再配布する場合は、[ASSET_NOTICE.md](ASSET_NOTICE.md)に従って権利を確認するか、利用可能な自分の素材へ差し替えてください。

相撲団体・選手等による公式提供や承認を示すものではありません。

## 改善・報告

不具合は環境、期待する動き、再現手順をIssueへ記載してください。機密情報は含めず、セキュリティの問題は [SECURITY.md](SECURITY.md) の非公開窓口を使ってください。コード・文書の投稿はMITで提供できるものに限り、第三者の権利表示を保持してください。動画の投稿には別途、出所と再配布条件の明示が必要です。
