# 🚨 JPFA緊急サイト GitHub Pages デプロイ手順

## ⚡ GitHub Pages で即座に公開（2分）

### 手順
1. **Settings** タブをクリック
2. 左メニューから **Pages** を選択  
3. **Source** で **Deploy from a branch** を選択
4. **Branch** で **main** を選択、フォルダは **/ (root)** のまま
5. **Save** をクリック

### 🌐 公開URL
数分後、以下のURLでサイトが公開されます：
**https://alohaloha.github.io/jpfa_test/**

## 🔄 更新方法

### ニュース追加
1. `index.html` を編集
2. ニュースセクションに以下を追加：
```html
<div class="news-item">
    <div class="news-date">● 2025.XX.XX</div>
    <div class="news-title">新しいニュースタイトル</div>
</div>
```

### スポンサー情報追加
1. `index.html` のスポンサーセクションを編集
2. 企業ロゴや名称を更新

### 緊急連絡先変更
1. `index.html` の `XXX-XXXX-XXXX` 部分を実際の電話番号に変更
2. 担当者名を更新

## 📞 Googleフォーム設定

### 1. フォーム作成
- [Google Forms](https://forms.google.com) で新規作成
- 質問項目: 名前、メール、問い合わせ種別、内容

### 2. フォーム連携
1. フォーム作成後、「送信」→リンクをコピー
2. `index.html` の以下を変更：
```javascript
// 変更前
alert('Googleフォームを設定してください...');

// 変更後  
window.open('https://forms.gle/あなたのフォームID', '_blank');
```

## 🎯 代替デプロイ方法

### Netlify（さらに簡単）
1. [Netlify](https://www.netlify.com) を開く
2. このリポジトリを connect
3. 自動デプロイ設定

### Vercel
1. [Vercel](https://vercel.com) でアカウント作成
2. GitHubリポジトリと連携
3. 自動デプロイ開始

## 🚨 緊急時の運用

### 即座に情報更新が必要な場合
1. GitHubで直接 `index.html` を編集
2. Commit changes で即座に反映
3. 数分で公開サイトに反映

### 大容量ファイル（画像等）
1. リポジトリに画像をアップロード
2. `index.html` で参照：`<img src="画像ファイル名.jpg">`

---

**🎉 これで JPFA緊急サイトがGitHub Pagesで公開されます！**
