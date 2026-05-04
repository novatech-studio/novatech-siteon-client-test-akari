# akari スタッフ写真 再生成指示書

## 共通ルール
- 全て写実的なAI生成写真（イラストNG）
- 正面顔は写さない（斜め後ろ・横顔シルエット・手元・肩越しのみ）
- 税理士事務所の清潔感ある空間（白・グレー・ウォームウッドトーン）
- 自然光または柔らかいオフィス照明
- テキスト・ロゴは入れない
- Shot with 85mm f/1.8 equivalent, candid moment, natural skin texture with visible pores
- 各画像を指定ファイル名で images/ に保存すること（WebP形式）
- 保存後に git add images/ && git commit -m "v2.0 スタッフ写真リアリティ改善（顔なし構図）" && git push を実行

## 画像一覧（4枚）

### 代表税理士 早瀬 恒一（大判・縦長）
- ファイル名: images/profile-hayase.webp（既存を上書き）
- サイズ: 1024x1792
- プロンプト: A senior Japanese male tax accountant seen from diagonally behind, sitting at a clean modern desk in a bright office. He is reviewing documents, natural light from window. Business suit, relaxed posture. No face visible. Shot with 85mm f/1.8, candid moment. Natural skin texture, no AI smoothing. Warm wood desk, white walls, subtle greenery.

### 税理士 篠崎 理央（正方形・小判）
- ファイル名: images/profile-shinozaki.webp（既存を上書き）
- サイズ: 1024x1024
- プロンプト: Close-up of a Japanese professional's hands holding a document in a bright modern office. Well-manicured hands, crisp white shirt cuff, document with text visible. Soft natural light, shallow depth of field, blurred office background. Shot with 85mm f/1.8. No face visible. Candid, natural.

### 税理士 水守 恒一（正方形・小判）
- ファイル名: images/profile-mizumori.webp（既存を上書き）
- サイズ: 1024x1024
- プロンプト: Side silhouette profile of a Japanese male professional in business attire, sitting at a desk in a bright modern office. Looking at a laptop screen, soft backlight from window creates gentle rim light. No direct face view. Shot with 85mm f/1.8. Clean minimal Japanese office aesthetic.

### スタッフ 名瀬 千紘（正方形・小判）
- ファイル名: images/profile-naze.webp（既存を上書き）
- サイズ: 1024x1024
- プロンプト: A Japanese professional woman seen from behind and slightly to the side, in a bright modern office. She is writing in a notebook on a clean white desk. Neat hair, professional blouse, natural light. No face visible. Shot with 85mm f/1.8. Warm, candid, natural texture. Minimal office background.

## index.html の更新が必要な箇所

画像生成・保存後、index.html 内の以下のパスを `.jpg` → `.webp` に変更すること:
- `images/profile-hayase.jpg` → `images/profile-hayase.webp` (2箇所)
- `images/profile-shinozaki.jpg` → `images/profile-shinozaki.webp`
- `images/profile-mizumori.jpg` → `images/profile-mizumori.webp`
- `images/profile-naze.jpg` → `images/profile-naze.webp`
