# cursor-driven-blueprint

これは、Cursor で課題を解決するためのフレームワークです。

このリポジトリは、自分の思考を整理し、複雑な問題を分解し、CursorのAI機能を効率的に活用するためのスターターキットを提供します。

## 🚀 クイックセットアップ

このフレームワークは、新規または既存のプロジェクトに対して、一度だけ行う初期設定として設計されています。

**ステップ1：フレームワークの設置**

自分のプロジェクトのルートディレクトリで、以下のコマンドを実行してください。これにより、フレームワークが `.cursor/blueprint` ディレクトリに設置されます。

```bash
# まず、設置先のディレクトリを作成します
mkdir -p .cursor

# 指定の場所にフレームワークをクローンします
git clone https://github.com/n4cl/cursor-driven-blueprint .cursor/blueprint
```

## 📖 実行フロー

このフレームワークを利用して、CursorのAIを活用しながらプロジェクトを進めるための基本的な流れを説明します。

### プロジェクトの開始

**目的:** プロジェクト全体の計画書 `.cursor/blueprint/plan.md` を作成する。

**手順:**
CursorのAgentチャットにて、以下のように指示をします。

> **あなたのプロンプト:**
> 「プロジェクトを開始します。
> `@.cursor/blueprint/project-flow.mdc を参考に、プロジェクトの計画を立てるための質問をしてください。」

**AIとの対話:**
AIが計画に必要な質問をしてくるので、それに答えていきます。対話が終わると、プロジェクトに必要なファイルが作成されます。

## 📁 ディレクトリ構造

```
.cursor/blueprint/
├── project/
│   ├── plan.md
│   ├── milestone-1/
│   │   ├── milestone.md
│   │   ├── task-001.md
│   │   └── ...
│   ├── milestone-2/
│   │   ├── milestone.md
│   │   └── ...
│   └── ...
├── README.md
├── templates/
│   ├── plan_template.md
│   ├── milestone_template.md
│   └── task_template.md
```

- **project/plan.md**: プロジェクト全体の目的・成果物・マイルストーン一覧。1プロジェクト1つ。
- **project/milestone-x/milestone.md**: 各マイルストーンの詳細（ゴール・完了条件・関連タスク一覧）。
- **project/milestone-x/task-xxx.md**: milestone.mdの完了条件を分解した最小単位のタスク。1タスク1ファイル。
- **templates/**: 各種テンプレート。
