# Claude Skills Hub

<div align="center">

![Claude Skills Hub](https://img.shields.io/badge/Claude-Skills%20Hub-blue?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Web-green?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)
![Version](https://img.shields.io/badge/Version-0.1.0-orange?style=for-the-badge)

**🤖 Claude Skills Hub - Claude スキルを発見・ダウンロード**

[![Live Demo](https://img.shields.io/badge/🌐-Live%20Demo-informational)](https://claudeskill.site)
[![Documentation](https://img.shields.io/badge/📚-Documentation-blue)](docs/)
[![Get Started](https://img.shields.io/badge/🚀-Get%20Started-success)](#はじめに)

</div>

## 言語 / Language

- [English](README.md)
- [中文简体](README_ZH.md)
- **日本語** (現在)
- [한국어](README_KO.md)
- [Français](README_FR.md)
- [Español](README_ES.md)

## 📋 プロジェクト概要

Claude Skills Hubは、Claudeユーザーに実用的なスキルテンプレートとツールを提供することを目的としたオープンソースのAIスキル共有プラットフォームです。このプロジェクトは、様々なClaudeスキルの収集、整理、共有に焦点を当て、ユーザーの作業効率向上を支援します。

### 🎯 プロジェクトの目標

- **📝 スキル収集**: 実用的なClaudeスキルテンプレートの収集と整理
- **🔧 ツール開発**: コード生成、文書作成などの実用的なツールの提供
- **📚 知識共有**: スキル共有と学習のためのコミュニティプラットフォームの構築
- **🚀 効率向上**: ユーザーが適切なAIスキルを迅速に見つけて使用できるよう支援

## ✨ 現在の機能

### 📖 スキルドキュメント
- **スキルテンプレート**: 標準化されたスキル記述フォーマット
- **使用ガイド**: 詳細なスキル使用説明と例
- **カテゴリ管理**: 機能領域別のスキル分類

### 🛠️ 基本ツール
- **文書生成**: 基本的な文書テンプレートとフォーマット
- **コード例**: 一般的なコードスニペットとテンプレート

### 🌍 コミュニティ構築
- **オープン貢献**: コミュニティ開発者によるスキルと改善の貢献を歓迎
- **文書標準**: 統一されたスキル文書規範の確立

## 📊 プロジェクト状況

<div align="center">

| 指標 | 現在の状態 | 説明 |
|------|------------|------|
| 📋 スキル数 | 3つの例 | ビジネス文書、UIコンポーネント、コードジェネレーター |
| 📂 スキルカテゴリ | 8カテゴリ | 開発、デザイン、ビジネスなど |
| 📚 文書完成度 | 基本版 | ユーザーガイドと開発者文書 |
| 🚀 プロジェクト段階 | 初期開発 | 貢献とフィードバックを歓迎 |

</div>

## 🎯 スキルカテゴリ

このプロジェクトは以下のカテゴリでAIスキルを整理し、現在はサンプルテンプレートを提供しています：

### 🔧 開発 (Development)
- **コードジェネレーター**: 各種プログラミング言語のコードテンプレート生成
- **API文書生成**: APIインターフェース文書の作成
- **テストコード**: ユニットテストとテストケースの生成

### 🎨 デザイン (Design)  
- **UIコンポーネント生成**: React/Vue/Angularコンポーネントテンプレート
- **デザイン文書**: デザイン仕様と説明文書

### 💼 ビジネス (Business)
- **ビジネス文書**: 事業計画書、提案書などの文書テンプレート
- **分析レポート**: データ分析とレポート形式

### 📝 コンテンツ (Content)
- **記事執筆**: ブログと技術記事のテンプレート
- **文書作成**: 技術文書と説明書

### 🎓 教育 (Education)
- **教材**: コースデザインと教育材料
- **学習ガイド**: 学習パスとチュートリアルテンプレート

*注：その他のカテゴリ（分析、研究、エンターテイメント）は計画中です。貢献を歓迎します。*

## 🚀 はじめに

### スキルの使用

1. **スキルの閲覧**
   - [claudeskill.site](https://claudeskill.site) にアクセスして利用可能なスキルを確認
   - `skills/` ディレクトリでスキル文書を確認

2. **スキルテンプレートの使用**
   - 対応するスキルのSKILL.md内容をコピー
   - 説明に従ってClaudeでスキルを使用

### 開発と貢献

1. **プロジェクトのクローン**
   ```bash
   git clone https://github.com/CavinHuang/claude-skills-hub.git
   cd claude-skills-hub
   ```

2. **新しいスキルの追加**
   - `skills/` ディレクトリに新しいスキルフォルダーを作成
   - 既存のフォーマットに従ってSKILL.md文書を作成

3. **貢献の提出**
   ```bash
   git add .
   git commit -m "feat: add new skill"
   git push origin feature/new-skill
   ```

## 🛠️ 技術アーキテクチャ

このプロジェクトはシンプルな静的ファイル構造を使用：

- **フロントエンド**: Next.js 14 + TypeScript
- **スタイリング**: Tailwind CSS
- **デプロイ**: Vercel
- **文書**: Markdown形式

## 📚 文書リソース

- **[ユーザーガイド](docs/user-guide.md)**: 使用説明とチュートリアル
- **[開発者文書](docs/developer-guide.md)**: 技術文書と開発ガイド
- **[貢献ガイド](CONTRIBUTING.md)**: プロジェクト貢献への参加方法

## 🤝 貢献ガイド

すべての形式の貢献を歓迎します！

### 貢献方法
- 🎯 新しいスキルテンプレートの追加
- 📝 既存文書の改善  
- 🐛 問題の修正
- 💡 機能の提案

### 貢献プロセス
1. プロジェクトリポジトリをフォーク
2. 機能ブランチを作成
3. 変更を提出
4. プルリクエストを作成

詳細な貢献ガイドラインについては、[CONTRIBUTING.md](CONTRIBUTING.md) を参照してください。

## 📄 ライセンス

このプロジェクトは [MIT ライセンス](LICENSE) の下でライセンスされています - 自由に使用、変更、配布してください。

## 🙏 謝辞

Claude Skills Hubに貢献してくださったすべての開発者に感謝します！

### 貢献者
- [@CavinHuang](https://github.com/CavinHuang) - プロジェクト作成者

### 特別感謝
- Anthropic Claudeチーム - AI技術サポートの提供
- オープンソースコミュニティ - インスピレーションと技術サポートの提供

## 📞 連絡先

- **🌐 ウェブサイト**: [https://claudeskill.site](https://claudeskill.site)
- **💬 ディスカッション**: [GitHub Discussions](https://github.com/CavinHuang/claude-skills-hub/discussions)
- **🐛 問題報告**: [GitHub Issues](https://github.com/CavinHuang/claude-skills-hub/issues)

---

<div align="center">

**⭐ このプロジェクトがお役に立てましたら、Starをお願いします！**

</div>