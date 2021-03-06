# Flow check

> **Part of the Multi-team Software Delivery Assessment** ([README](README.md))
> 
> Copyright © 2018-2019 [Conflux Digital Ltd](https://confluxdigital.net/)
> 
> Licenced under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) ![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/3.0/88x31.png)
>
> _Permalink: [SoftwareDeliveryAssessment.com](http://SoftwareDeliveryAssessment.com/)_ 

Nicole Forsgren氏、Jez Humble氏、Gene Kim氏の書籍  [_Accelerate_](https://itrevolution.com/book/accelerate/) の評価基準に基づき作成し、Don Reinertsen 氏の書籍 [_The Principles of Product Development Flow_](https://www.amazon.com/Principles-Product-Development-Flow-Generation/dp/1935401009) から、いくつかチェック項目を追加しました。

目的：*E2Eのリリースメトリクスに関するチームの認識とパフォーマンスを評価すること*

方法：[Spotify Squad Health Check](https://labs.spotify.com/2014/09/16/squad-health-check-model/) のアプローチを使用して、次の質問に対するチームの回答を評価する:   

| **質問**                                                                                                                                                                    | **しんどい (1)**                                                              | **すばらしい (5)**                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1\. **サイクルタイム** - コードの変更がバージョン管理からプロダクションで実行されるまでどのくらいかかりますか？ （最小、標準）                                           | 2週間以上                                                         | 1時間以内                                                                                                                                      |
| 2\. **デプロイ頻度** - チームは本番環境にどのくらいの頻度でデプロイしますか？                                                                                                 | 2週間ごとか、それ以上                                        | 2日ごとか、それ以下                                                                                                                              |
| 3\. **MTTR** - インシデント後、アプリケーションまたはサービスを復元するのにどれくらい時間がかかりますか？                                                                             | わからない - MTTRを計測していない                                | MTTRを計測し、10分で自動的にサービスを復元し、これをデプロイメント・パイプラインでテストする                              |
| 4\. **失敗した変更** - 本番環境でのアプリケーションまたはサービスの変更が、どの程度の割合で失敗するか、修正が必要ですか？ （これは通常、失敗したデプロイの数になります。）| 本番環境での変更/デプロイの20％以上が失敗する  | 本番環境での変更/デプロイの5％未満が失敗する|
| 5\. **タスクキューの長さ** - あなたのチームは同時にいくつの仕事をしていますか？ （最小、標準）                                                                         | チームメンバーよりもかなり多くの作業中（WIP）のアイテムがあります。| 待ち行列理論（または遅延コスト）に基づいて明示的にWIPを制限した。WIPはチーム内の人数以下である |
| 6\. **イノベーション** - デプロイ手段をどの程度新しい技術を取り入れ改善できますか？                                                                                      | 新しい技術を取り入れる時間はない                | 毎週、デプロイの改善のための時間を確保し、チーム指標の一部として進捗状況を確認する                                           |
| 7\. **オンボーディング** - 新しいチームと新しいスタッフのオンボーディングプロセスはどの程度効果的ですか？                                                                                    | オンボーディングプロセスは信じられないほど困難で、進歩を妨げる | オンボーディングプロセスは、非常にシンプルでわかりやすい                                                                              |
| 8\. **Branchの寿命** - ブランチはどれくらいの期間存在しますか？ （*Master*以外）                                                                                                  | 機能ブランチは多くのスプリントで持続する           | Mater/Trunkで直接開発し、機能ブランチの寿命は2日以内である                                                             |
| 9\. **ふりかえり** - チームのふりかえりはどの程度効果的ですか？                                                                                                           | 定期的なふりかえりはありません                | ふりかえりは、チームが本当にエンゲージされ、価値があり、効果的だ                                              |
