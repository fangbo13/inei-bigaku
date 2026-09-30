# 人物の陰翳 —— 詳細仕様

SKILL.md §4 の補足。人物が写っている写真では必ず読む。

## 目次
1. なぜ人物はホラーになりやすいのか
2. 光の配置と比率
2b. 人と空間を一体にする
3. 肌・目・身体の言葉（入れるもの／入れないもの）
4. 撮り方A：光だけを変える（既定）
5. 撮り方B：寄りの切り取り
6. 撮り方C：映画の一場面として再構成
7. 症状別の修正
8. ユーザーへの一言の例

---

## 1. なぜ人物はホラーになりやすいのか

| 原因 | 画像モデルの連想 | 対策 |
|---|---|---|
| 暗闇に顔だけが浮かぶ | 生首、怨霊、J-ホラー | 衣と肩の形を闇の中にかすかに残す、背景に空間の気配 |
| 下からの光、正面からの光 | 懐中電灯の怪談、不気味な演出 | 光は横から45°、目の高さかやや上から |
| 青白い・灰色の肌 | 死体、幽霊 | 1800〜2500K の暖色、肌の次表面散乱 |
| 顔の半分が真っ黒 | 欠けた顔、不気味の谷 | 影の側にも階調を残す（光の側の1/4〜1/8） |
| 目に光がない | 虚ろな目、死んだ目 | 瞳に小さなキャッチライトひとつ |
| 粒子・汚し・経年感を顔に当てる | 汚れた肌、腐敗、病 | 肌はなめらかに。質感は衣と器に置く |
| 無表情の正面アップ | 呪いの写真 | 横顔、伏し目、しぐさ、または表情は元のまま光で和らげる |

谷崎の随筆には、昔の女性が眉を落とし歯を染め、暗い衣で身体を闇に沈めて、顔だけを仄白く浮かばせたという話が出てくる。文学としては幽玄の極みだが、**これを画像でそのまま再現してはいけない**。現代の画像モデルとそれを見る人の目には、ほぼ確実に怪談として読まれる。取り入れるのは「人を闇の空間の一部として見る」という見方だけにする。

## 2. 光の配置と比率
2b. 人と空間を一体にする

- **キーライト**：ひとつ。被写体の横45°前後、目の高さか少し上から。蝋燭・行灯・窓からの夕光の暖色（1800〜2500K）。障子越しの外光を使うときも、肌に当たる部分はやや暖かく寄せる。
- **明暗比**：光の側：影の側 = 4:1〜8:1。影の側の目鼻は、目を凝らせば読めるように。
- **リムライトは控えめに**：光の当たる側の髪か肩の、ごく短い一部分だけ。輪郭全体を光で縁取ると、背景から切り離された切り抜き写真になる。影の側の輪郭は背景の闇に溶かす（§2b）。
- **背景**：真っ黒にせず、キーライトがわずかに届く壁・屏風・窓枠・柱の気配を残す。人が「どこかの部屋にいる」と分かること。
- **下からの光・真正面からの光・フラッシュ**は使わない。

## 2b. 人と空間を一体にする

撮り方Aで起きやすい失敗は、元写真の光のまま残った人物が、描き直された背景の上に貼り付いたように見えること。原因は、「人物を変えるな」という指示をモデルが「人物のピクセルに触れるな」と解釈することにある。

| 手段 | 指示文に使う言葉 |
|---|---|
| 同一性と光を切り分ける | `Preserve the person's identity (facial structure, features, expression, age, hairstyle), but completely re-render the lighting, shadows and color on the person to match the room.` |
| 一つの光が人と部屋を照らす | `The same single {lamp} at {position} lights both the wall behind and the person's cheek, with the same direction, color temperature and falloff.` |
| 影の側を背景に溶かす | `On the shadow side, the person's silhouette merges into the background darkness of equal value — lost edges, no outline separating the figure from the room.` |
| 落ち影・接地影 | `The person casts a soft shadow onto the wall / floor; contact shadows under the hands and the cup.` |
| 照り返し | `A faint warm bounce light from the nearby wooden wall on the shadow side of the face.` |
| 同じ光だまり | `The person and {the table / the cup / the tatami} share the same small pool of light.` |
| 同じ空気 | `The same film grain, color grade, depth of field and faint atmospheric haze over both the person and the room.` |
| 合成感の否定 | `Not a composite, not a cutout, no halo around the figure, no studio rim light outlining the silhouette.` |

**二段階の作り方**（Gemini は会話の中で続けて編集できるので有効）
1. 一段目：人物ごと空間全体を一つの光で描き直す。顔立ちが多少揺れてもよいとし、一体化を優先する（§4 の雛形）。
2. 二段目：元写真をもう一度添えて、`Keep this lighting, shadows, color and atmosphere exactly as they are. Only restore the person's facial features to match the original photo.` のように、顔立ちだけを戻す。

## 3. 肌・目・身体の言葉

**入れる**
```
warm subsurface scattering in the skin, a faint reddish glow at the edge of the ear, cheekbone and fingertips,
soft amber / honey key light (about 2000K) from the side, gentle skin falloff, smooth healthy skin,
shadow side of the face still readable with soft detail,
the person lit by the same light as the room, soft cast shadow on the wall, contact shadows, faint warm bounce light,
a small warm catchlight in the eyes,
the garment and shoulders faintly readable in the darkness, the shadow side of the figure merging into the room,
the room faintly visible behind the person,
calm, tender, meditative mood, alive and warm
```
**入れない（否定語に回す）**
```
pale skin, grey skin, cold light, bluish tint, uplighting, flashlight, harsh half-black face,
floating head, disembodied face, eerie, ghostly, horror, J-horror, sinister, mournful, hollow eyes,
dirty skin, blotchy skin, aged texture on the face, heavy grain on the face,
composite, cutout, pasted-in figure, halo around the figure, studio rim light outlining the silhouette, person lit differently from the background
```

## 4. 撮り方A：光だけを変える（既定）

その人らしさに意味がある写真（家族、本人、大切な人）に使う。似ていることを優先しつつ、人と空間を一体にする（§2b）。

```
Re-light this whole photograph — the person and the room together — in the aesthetic of Tanizaki's "In Praise of Shadows", as a quiet cinematic still.

Identity: preserve the person's identity — facial structure, features, expression, age, hairstyle, pose and framing.
But do not preserve the original lighting on the person: completely re-render the light, shadows and color on the person so they belong to the new room light. The person and the room must look like one photograph taken under one light, not a composite.

Light: one single soft, warm light (about 2000K, like a paper lantern) placed {e.g. "low on the left, just off frame"}. This same light falls on {e.g. "the wooden wall behind"}, on the person's cheek and hands, and on {e.g. "the table and the cup"}, with the same direction, color and inverse-square falloff. Light-to-shadow ratio about 6:1.
Shadow side: the shadow side of the face stays readable with soft detail; the shadow side of the body and hair merges into the background darkness of equal value — lost edges, no outline around the figure. Only a short stretch of the lit-side edge catches light.
Interaction: the person casts a soft shadow on {the wall / the floor}; contact shadows under the hands; a faint warm bounce from {the wall / the tatami} on the shadow side of the face.
Skin: smooth, healthy and warm, gentle subsurface scattering at the ear, cheekbone and fingertips. No pale or grey tones. A small warm catchlight in the eyes.
Room: {keep the original room}, re-lit by the same light — most of it sinks into warm darkness, a few surfaces faintly visible.
Atmosphere: the same very fine grain, color grade, depth of field and faint haze over the person and the room.
Tone: low-key, about 70% of the frame in shadow with rich gradation of soot-brown and lacquer-black; highlights honey and ivory, never white.
Mood: calm, tender, contemplative, alive.
Avoid: composite or cutout look, halo or rim-light outline around the figure, the person lit differently from the room, horror, ghostly pale face, floating head, dirty or blotchy skin, beauty-filter plastic skin, added props.
```
**日本語要約**：人物ごと部屋全体を一つの行灯の光で照らし直す。顔立ち・表情・構図は保つが、人物に当たる光は元のまま残さない。影の側の身体は背景の闇に溶かし、輪郭を光で縁取らない。壁への落ち影、手の下の接地影、壁からの照り返しで、人と空間をつなぐ。

顔立ちが揺れた場合は、§2b の二段目の指示で顔だけを戻す。

## 5. 撮り方B：寄りの切り取り

```
Crop closely to {e.g. "the lowered eyelids and the cheek" / "the hands holding the tea bowl" / "the nape of the neck and the collar"}; the rest of the person and the room dissolve into warm darkness, with the silhouette still faintly sensed.
{Light and skin: same as Pattern A.}
Visual anchor: {e.g. "steam rising from the bowl between the fingers, catching the light" / "the warm translucent glow at the fingertips"}.
```
手元・器・湯気の組み合わせは、人物の陰翳でもっとも失敗が少なく、もっとも陰翳らしい。元写真に手が写っていれば、まずこれを提案するとよい。

## 6. 撮り方C：映画の一場面として再構成

顔立ちの同一性は保証できないので、ユーザーの同意を得るか、再解釈を求められたときに使う。

| 型 | 指示文の核 | 手本 |
|---|---|---|
| **横顔** | `the person in profile; the bridge of the nose, the lips and the chin traced by a thin line of warm golden light; the rest of the face in soft shadow` | 杜可風（王家衛『花様年華』）、フィリップ・ル・スール（『グランド・マスター』） |
| **後ろ姿** | `seen from behind, seated by a shoji window / a folding screen, facing away, the garment merging into darkness, the gaze lost in the dim space` | ヴィルヘルム・ハンマースホイ |
| **しぐさ** | `the person pouring tea / arranging flowers, face turned down and half in shadow, the hands and the vessel carrying the light` | 李屏賓（侯孝賢『黒衣の刺客』）の燭光の室内 |
| **空間の中の小さな人** | `a small figure deep in a dark room, lit only by a distant window, the architecture holding most of the frame` | 宮川一夫、ハンマースホイ |

人は画面の主人公ではなく、暗い空間の一部として置く。

## 7. 症状別の修正

| 症状 | 追加指示 |
|---|---|
| ホラー・幽霊っぽい | `Make it warm and alive: warmer skin with subsurface glow, add a catchlight in the eyes, let the garment and shoulders be faintly readable, reveal the room faintly behind. Calm and tender mood.` |
| 生首に見える | `Connect the head to the body: let the neck, shoulders and garment folds be faintly readable in the same warm light; do not let the body disappear completely.` |
| 人物が浮いている・切り抜き合成に見える | `The person looks pasted in. Re-render the light on the person so it comes from the same {lamp} as the room: same direction, color and falloff. Merge the shadow side of the figure into the background darkness, remove any outline or halo, add a soft cast shadow on the wall and contact shadows, and apply the same grain and haze to both.` そのうえで必要なら §2b の二段目で顔立ちを戻す |
| 顔色が悪い・灰色 | `Warm the skin toward honey and amber; add gentle subsurface scattering at the ears and cheeks; remove grey and blue tones.` |
| 顔が汚れて見える | `Smooth, clean, healthy skin; remove texture and grain from the face; keep the aged texture only on the garment and background.` |
| 本人に似ていない | `Keep the face identical to the original photo; change only the lighting.` |
| 美顔フィルターのようにのっぺりした | `Natural skin with real pores, not airbrushed; keep the low-key mood.` |

## 8. ユーザーへの一言の例

> おばあさまの表情はそのままに、お部屋ごと行灯のような温かい一灯で照らし直し、お姿が部屋の暗がりに自然に溶けるようにしました。美肌の肖像ではなく、静かな映画の一場面のような画です。湯呑みを持つ手元に寄った版もお作りできます。

> 正面のお写真なので、顔立ちを保つために光だけを変えています。横顔や後ろ姿の「映画の一場面」として大きく描き直すこともできますが、その場合はお顔が変わる可能性があります。
