# UiPath Learning

2026年10月9日〜12月31日に、UiPath Certified Professional Automation Developer Associateの合格を目指す学習リポジトリです。公式の無料教材を軸に、自作演習と検証結果をGitへ保存します。

## 最初に開くページ

| 用途 | ページ |
|---|---|
| 全体の予定・48タスクの索引 | [工程表](docs/schedule.md) |
| 着手・進捗・完了の管理 | [GitHub Issues](https://github.com/akihitot/uipath-learning/issues) |
| 日本語で基礎を理解する | [日本語学習ガイド](docs/japanese-guide.md) |
| 日次記録と毎週金曜の振り返り | [学習記録](docs/learning-log.md) |
| 模試・受験の記録方法 | [模試・受験記録](docs/exam-log.md) |
| 制作テーマ候補10個 | [制作テーマ](docs/robot-themes.md) |

工程表は予定の正本、Issuesは進捗の正本です。以前のExcel工程表を毎日並行更新する必要はありません。日本語ガイドは独自の補助教材で、公式教材の全文翻訳ではありません。

## 現在地と次の作業

2026/10/10時点で、Studio Communityの導入、メッセージボックスの実行、Git設定、初回コミット、GitHubへの保存を確認済みです。試験は未受験・資格は未合格。実績時間は未記録です。

1. [T01 / #1](https://github.com/akihitot/uipath-learning/issues/1)を開き、Academyへの登録と現行試験仕様・無料機能の確認を行う。
2. [T02 / #2](https://github.com/akihitot/uipath-learning/issues/2)でRPAと製品の役割を学ぶ。
3. [T03 / #3](https://github.com/akihitot/uipath-learning/issues/3)で変数・引数を実習し、[T04 / #4](https://github.com/akihitot/uipath-learning/issues/4)で分岐・繰り返しへ進む。

## 学習を進める手順

1. 工程表から今週のIssueを開き、「着手日」をコメントする。
2. 公式単元を受講し、日本語ガイドと自作演習で確認する。
3. 期待結果・実結果・実績時間・困り事をIssueにコメントする。
4. 下記のGit保存を行い、コミットURLをIssueへ残す。
5. 完了条件を満たしたらチェックを付け、「Close issue」で閉じる。
6. 毎週金曜に予定と残作業を確認し、繰越はIssueの期限と工程表を更新する。

```powershell
git pull --ff-only
# Studioで演習を作成・保存した後
git add .
git status
git commit -m "T03：変数と引数の演習を追加"
git push
```

変更がないときはコミット不要です。公開前にgit statusと差分を確認します。

## 最初の演習を再現する

- Windows用プロジェクト、式の言語はVB.NET。
- 作成時：Studio 2026.0.203、UiPath.System.Activities 26.8.2。
- GitHubからcloneし、Studioでルートのproject.jsonを開く。依存関係の復元が完了してからMain.xamlを実行する。
- 期待結果：「UiPathの動作確認ができました」というメッセージが表示される。

```powershell
git clone https://github.com/akihitot/uipath-learning.git
```

現在はAssociateBasicsプロジェクトがリポジトリのルートにあります。新しい実習A/Bは別のStudioプロジェクトとしてrobots/lab-a、robots/lab-bへ作成する予定です。まだ作成していません。

## 学習の基準

- [公式Academyコース](https://academy.uipath.com/ja/learning-plans/automation-developer-associate-training)
- [公式認定資格FAQ](https://www.uipath.com/ja/learning/certification/faqs)
- [Studioドキュメント](https://docs.uipath.com/studio)

2026/10/10確認時のAcademyコースはv2024.10・英語。インストール済みStudioは2026版なので、画面・アクティビティ名の違いを記録します。初回受験は12/4が目標で、予約済みではありません。予約・支払いは本人が行います。

学習資料と演習は初期無料を基本とし、受験料は別途必要です。資格合格は公式結果で判定します。

## 保存する内容

自作ワークフロー、架空サンプル、期待値、検証結果、説明資料を保存します。認証情報、本人確認情報、試験結果原本、公式模試・本試験の問題文は保存しません。リポジトリは現在Publicです。レビュー依頼や共同作業への招待は必要になった時点で行います。
