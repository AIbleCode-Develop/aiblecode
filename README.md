# AIbleCode

## 技術スタック

#### フロントエンド技術

<p style="display: inline">
    <img src="https://img.shields.io/badge/TypeScript-gray?logo=typescript" alt="TypeScript"/>
    <img src="https://img.shields.io/badge/React-gray?logo=react">
    <img src="https://img.shields.io/badge/TailwindCSS-gray?logo=tailwindcss" alt="TailwindCSS"/>
</p>

#### バックエンド技術

<p style="display: inline">
    <img src="https://img.shields.io/badge/Next.js-gray?logo=nextdotjs" alt="Next.js"/>
    <img src="https://img.shields.io/badge/MySQL-gray?logo=mysql" alt="MySQL"/>
</p>

#### インフラ技術

<p style="display: inline">
    <img src="https://img.shields.io/badge/AWS Amplify-Gen 2-blue?logo=awsamplify" alt="AWS Amplify"/>
</p>

## セットアップ

<!-- TODO: セットアップ方法を記述する -->
// あとで作成します

## ブランチ戦略

- **mainブランチ** （`main`）
  - 本番にデプロイするモジュールを作成するメインとなるブランチ

- **hotfixブランチ** （`hotfix`） 
  - 致命的なバグが発生した際に緊急で修正を加えるためのブランチ
  - `main`ブランチと進行中の`release`ブランチに変更をマージする

- **releaseブランチ** （`releace/?`）
  - リリース対象の変更がマージされたブランチ
  - `main`ブランチから作成され、リリースのタイミングで`main`ブランチにマージ、削除される
  - 開発環境でのテストに使用する
  - Github Flowの統合ブランチと似た用途だが、リリースごとに１つという特性がある

- **featureブランチ** （`feature/?/?`） 
  - 機能開発を行うブランチ
  - `release`ブランチから派生し、`release`ブランチのマージ時点で削除する

<img src="docs/images/branch-strategy.png">

参考資料：[Zenn：小規模チーム開発のブランチ戦略を考える（GitHub Flowベース）](https://zenn.dev/gnz/articles/6674530f61cfbe)

## 貢献ガイドライン

- 新しい機能は`feature`ブランチで開発してください。
- バグ修正は緊急度に応じて`hotfix`ブランチで行います。
- プルリクエストは小さい単位で出し、必ずコードレビューを受けてからマージします。

## ライセンス

本プロジェクトは **MIT License** の元で行います。詳細は [LICENSE](LICENSE) を参照してください。
