トレーニングログ Ver.1.01 / iPhone向け導入手順

【ファイル】
index.html
service-worker.js
manifest.webmanifest
icon-180.png
icon-192.png
icon-512.png

【GitHub Pagesへの配置】
1. ZIPを展開し、上記6ファイルを同じフォルダに配置します。
2. GitHubリポジトリのルートに6ファイルをアップロードします。
3. Settings > Pages > Deploy from a branch で公開します。
4. 公開URLをiPhoneのSafariで開きます。
5. 共有ボタン > ホーム画面に追加 > 追加 を選択します。

【Ver.1.01の変更点】
・部位に「上半身」「下半身」を追加
・指定7種目を追加
・各種目10セットまで記録可能
・レップ数を数字入力に変更
・RPEを削除
・分析期間を開始日～終了日で指定可能
・選択種目の重量推移をレップ数加重平均に変更
  平均使用重量 = 各セットの（重量×レップ数）の合計 ÷ レップ数の合計
・ベンチプレス専用グラフを削除
・端末設定に合わせる／ライト／ダークのテーマ切替
・Service Workerキャッシュをv3に更新
・旧バージョンの5セット記録・履歴データを引き継ぎ

【注意】
・既存履歴は同じブラウザ・端末のlocalStorageに保存されています。更新前に「履歴」画面の「バックアップ出力」を実施してください。
・アプリを公開した後、古い表示が残る場合はSafariでページを再読み込みしてください。Service Workerが新しいキャッシュへ切り替わります。
・PWAはHTTPSまたはlocalhostでのみ有効です。
・OneDrive/SharePointのファイルプレビューではService WorkerとlocalStorageが制限される場合があります。
・SafariのWebサイトデータ削除やアプリ削除に備え、バックアップを定期的に出力してください。
