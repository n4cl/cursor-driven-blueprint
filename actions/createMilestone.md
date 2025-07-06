# createMilestone アクション詳細

## 概要
マイルストーン詳細（milestone-x/milestone.md）を作成するアクション。

## 実行ルール
1. ユーザーとの対話の最初に、以下の提案を行う：
    > **AIからの提案:**
    > 「全体計画 `plan.md` はありますが、現在取り組むマイルストーン `milestone-x/milestone.md` が未設定です。
    > どのマイルストーンから詳細化しますか？
    > マイルストーン名を教えていただければ、`templates/milestone_template.md` を参考にして、私が `milestone-x/milestone.md` を作成します。」
2. ユーザーからマイルストーン名・内容を受け取った後、テンプレートに沿って詳細をヒアリングし、`milestone-x/milestone.md` を作成する。
