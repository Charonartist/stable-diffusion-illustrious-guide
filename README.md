# Stable Diffusion Illustrious プロンプトガイド

## 基本的なプロンプト構造
Illustriousモデルでは、以下の順序でプロンプトを記述することが推奨されています：

1. キャラクター説明
2. スタイル指定
3. シーンや状況の説明
4. 品質や技術的な指定

## プロンプトの書き方のポイント

### 1. 基本原則
- 明確で簡潔な言語を使用する
- Danbooru形式のタグを活用する
- 具体的すぎる指定は避ける
- 画像の要素を順序立てて記述する

### 2. 推奨設定
- サンプラー：Euler a/SGM
- CFG Scale：4-6の範囲
- 必要に応じてネガティブプロンプトを活用

### 3. プロンプトの構成要素

#### キャラクター要素
- 外見的特徴（髪型、服装、表情など）
- ポーズや動作
- 感情表現

#### スタイル要素
- アートスタイル（デジタルアート、油彩など）
- 参照元（artstation, conceptartなど）
- 色調やムード

#### 技術的要素
- 解像度（4k, 8kなど）
- レンダリング品質（highly detailed, sharp focusなど）
- ライティング（cinematic lighting, soft lightingなど）

## プロンプト例文

### 基本的な例
```
1girl, blue hair, casual wear, gentle smile --style digital art, anime, detailed --outdoor scene, cherry blossoms, spring day --highly detailed, 4k, sharp focus
```

### 詳細な例
```
1girl, long flowing hair, elegant dress, detailed face, expressive eyes --style masterpiece, digital painting, anime style --magical forest background, mystical atmosphere, glowing particles --ultra detailed, cinematic lighting, artstation quality, 8k
```

## ネガティブプロンプト活用のヒント

1. まずネガティブプロンプトなしで生成
2. 不要な要素が出現した場合に追加
3. 一般的に避けたい要素：
   - 低品質要素（low quality, blurry, watermark）
   - 不要なノイズ（grain, noise）
   - 構図の乱れ（bad anatomy, extra limbs）

## トラブルシューティング

### よくある問題と解決方法

1. 構図が崩れる場合
   - キャラクターの位置や向きを具体的に指定
   - 基本的な構図用語を追加（portrait, full body, close-upなど）

2. スタイルが安定しない場合
   - スタイル指定を先頭に持ってくる
   - 参照元となるアーティストやメディアを指定

3. 細部の品質が低い場合
   - detailed, high quality などの品質指定を追加
   - CFG Scaleを調整

## 参考リソース

1. モデルの入手先
   - Civit
   - Hugging Face

2. UIの設定
   - AUTOMATIC1111推奨
   - 基本設定の確認と調整

## アップデート情報

最終更新：2024年12月
- 最新バージョンの特徴と変更点の確認
- 新しいプロンプト手法の追加
- コミュニティからのフィードバック反映

## 注意点

1. モデルの特性
   - アニメ調の画像生成に特化
   - Danbooru形式のタグシステムを採用
   - 品質設定の影響が大きい

2. 制限事項
   - 極端に複雑なシーンは苦手
   - 特定のスタイルに偏る可能性
   - プロンプトの順序が重要