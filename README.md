# AIbleCode

## 技術スタック

### フロントエンド技術

<p style="display: inline">
    <img src="https://img.shields.io/badge/TypeScript-gray?logo=typescript" alt="TypeScript"/>
    <img src="https://img.shields.io/badge/React-gray?logo=react">
    <img src="https://img.shields.io/badge/TailwindCSS-gray?logo=tailwindcss" alt="TailwindCSS"/>
</p>

### バックエンド技術

<p style="display: inline">
    <img src="https://img.shields.io/badge/Next.js-gray?logo=nextdotjs" alt="Next.js"/>
    <img src="https://img.shields.io/badge/MySQL-gray?logo=mysql" alt="MySQL"/>
</p>

### インフラ技術

<p style="display: inline">
    <img src="https://img.shields.io/badge/AWS Amplify-Gen 2-blue?logo=awsamplify" alt="AWS Amplify"/>
</p>

## ブランチ戦略
- **mainブランチ** （`main`）
  - 本番にデプロイするモジュールを作成するメインとなるブランチ

- **hotfixブランチ** （`hotfix`） 
  - 致命的なバグが発生した際に緊急で修正を加えるためのブランチ
  - mainブランチと進行中のreleaseブランチに変更をマージする

- **releaseブランチ** （`releace/?`）
  - リリース対象の変更がマージされたブランチ
  - mainブランチから作成され、リリースのタイミングでmainブランチにマージ、削除される
  - 開発環境でのテストに使用する
  - Github Flowの統合ブランチと似た用途だが、リリースごとに１つという特性がある

- **featureブランチ** （`feature/?/?`） 
  - 機能開発を行うブランチ
  - releaseブランチから派生し、releaseブランチのマージ時点で削除する

<img src="docs/images/branch-strategy.png">

参考資料：[Zenn：小規模チーム開発のブランチ戦略を考える（GitHub Flowベース）](https://zenn.dev/gnz/articles/6674530f61cfbe)

## ライセンス

本プロジェクトは **MIT License** の元で行われます。詳細は [LICENSE](LICENSE) を参照してください。
