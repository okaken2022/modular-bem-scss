# modular-bem-scss

モダンでスケーラブルな Sass/SCSS テンプレート。6-1 パターンアーキテクチャと BEM メソドロジーを採用し、保守性の高い CSS コードベースを実現します。

A modern and scalable Sass/SCSS template implementing the 6-1 pattern architecture and BEM methodology for maintainable CSS codebase.

## 特徴 / Features

- 📁 6-1 パターンアーキテクチャ / 6-1 Pattern Architecture
- 🎨 BEM メソドロジー / BEM Methodology
- 🧩 モジュラーコンポーネント設計 / Modular Component Design
- 🛠 ユーティリティファーストアプローチ / Utility-First Approach

## ディレクトリ構造 / Directory Structure

```
sass/
│
├── abstracts/      # 変数、関数、ミックスイン
│                   # Variables, functions, mixins
│
├── base/           # リセット、基本スタイル
│                   # Reset and base styles
│
├── components/     # 再利用可能なコンポーネント
│                   # Reusable components
│
├── layout/         # レイアウト要素
│                   # Layout elements
│
├── pages/          # ページ固有のスタイル
│                   # Page-specific styles
│
├── utility/        # ユーティリティクラス
│                   # Utility classes
│
└── style.scss      # メインのSassファイル
                    # Main Sass file
```

## 命名規則 / Naming Convention

BEM メソドロジーに基づく命名規則を採用しています。  
Following BEM methodology for class naming:

```scss
.block {
  &__element {
    // Element styles
  }

  &--modifier {
    // Modifier styles
  }
}
```

### 例 / Example

```html
<div class="card">
  <div class="card__header">
    <h2 class="card__title">Title</h2>
  </div>
  <div class="card__content">
    <p class="card__text">Content</p>
  </div>
  <div class="card__footer card__footer--highlighted">
    <button class="button button--primary">Action</button>
  </div>
</div>
```

## ユーティリティクラス / Utility Classes

主要なユーティリティクラスの例：  
Examples of key utility classes:

```scss
.u-margin-top--small {
  margin-top: 1rem;
}
.u-padding-x--medium {
  padding: 0 2rem;
}
.u-text-center {
  text-align: center;
}
```

## カスタマイズ / Customization

1. `abstracts/_variables.scss`で基本設定をカスタマイズ  
   Customize base settings in `abstracts/_variables.scss`

2. 必要に応じてコンポーネントを追加・修正  
   Add or modify components as needed

3. ユーティリティクラスは`utility/`ディレクトリで管理  
   Manage utility classes in the `utility/` directory

## ベストプラクティス / Best Practices

1. コンポーネントの独立性を保つ  
   Keep components independent

2. ユーティリティクラスは慎重に追加  
   Add utility classes thoughtfully

3. 一貫した命名規則を維持  
   Maintain consistent naming conventions

4. 適切なコメントを追加  
   Add appropriate comments
