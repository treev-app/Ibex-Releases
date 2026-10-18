# Ibex for macOS

Ibex（アイベックス）は、オンライン通話の画面と音声をMP4に保存し、無料の端末内AIで日本語の議事録を作成するmacOSアプリです。

## ダウンロード

[最新版のIbexをダウンロード](https://github.com/treev-app/Ibex-Releases/releases/latest)

このリポジトリはIbexの公式配布専用です。GitHub Releaseには次のファイルだけを掲載します。

- `Ibex-*-arm64.dmg`: Apple Silicon搭載Mac用インストーラー
- `Ibex-*-arm64.dmg.sha256`: 改ざん確認用のSHA-256チェックサム

## インストール方法

1. 最新リリースからDMGをダウンロードします。
2. DMGを開き、Ibexを「Applications」フォルダへドラッグします。
3. ApplicationsフォルダからIbexを起動します。
4. macOSに求められたら、画面収録・システムオーディオ・マイクを許可します。

配布DMG内のアプリはDeveloper IDで署名し、Appleの公証を通過したものだけを公開します。

## チェックサムの確認

DMGと同じリリースにある`.sha256`ファイルをダウンロードし、ターミナルで次を実行します。

```bash
shasum -a 256 -c Ibex-1.3.5-arm64.dmg.sha256
```

バージョン番号はダウンロードしたファイルに合わせて変更してください。`OK`と表示されれば一致しています。

## プライバシーと録画の同意

標準設定では、録画・文字起こし・議事録をMac内で処理します。録画を開始する前に、必ず参加者全員へ目的を説明し、同意を得てください。

不具合は[Issues](https://github.com/treev-app/Ibex-Releases/issues)へお知らせください。脆弱性の報告は公開Issueへ書かず、[Security](SECURITY.md)の案内をご利用ください。
