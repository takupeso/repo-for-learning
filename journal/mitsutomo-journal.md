# Jounal
## 2026-5-25
### Git, GitHub Learning Session
- 学んだこと
    - GitHubとLocalのEditorの役割の違い
    - Localで編集した後のRemoteの取り回し
    - Remoteが更新されたあとのLocalへの取り込み
- これがなぜ重要か
    - 個人作業であっても、チームの共同作業であっても、何を・なぜ変えたのかTrackできること
    - Local環境で作業することで、手元のネットワーク環境やお互いの更新内容に影響を受けず作業できる
    - WordやGoogle Docs、Notionでの管理の場合、魚拓を取るなどしないとTrack changeが大変。また、なぜ変更したのかは残しにくい
- これからどうするか
    - GitHubはみんなが合意した状態のDocument置き場的なもの。
    - Codeなら、CI/CDパイプラインを設定してAWSなどにデプロイ。
    - Document置き場から実際に頻繁に参照するDocumentハブとするにはどうするか。特に、非エンジニアにとっては読みにくい。
        - GitHub Actionsで自動でHTMLなどにして、Github PagesやAWS S3などにおく。
        - NotoinやConfluenceをHubとして当該リンクを貼っておく。など
- 感想や疑問
    - Terminal操作やGitのインストールは、結局根本を理解しないままやった形なので、そこも深堀すべきかな。。
    - GitHubでConflictが起こるようなBranchのマージが起こるときに、Reviewするの大変そう
    - 自分の理解もまだまだなので、これを浸透させていくにはかなり大きな壁がありそう。
        - クラウド上での共同編集と比べると変更点のシンクがPull RequestのReview、Mergeになるので同期は取りづらい
        - 一方で、「コメント→解決」あるいは「直接Edit」と比べると、誰のどんな思いが反映されていったかは残しやすいナー
