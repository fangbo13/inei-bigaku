# 光学・色の仕様

陰翳の美学を、画像モデルが理解できる光学・レンダリング・撮影の言葉と数値に置き換えるための参照表。
**生成の指示文には、ここの英語の言葉を使う。** 日本語の美学語彙は判断のためのもので、指示文には入れなくてよい（入れる場合も光学の言葉と併記する）。

## 目次
1. 文学 → 光学 対照表
2. 素材別のレンダリング語
3. 刺点のレンダリング語
4. 明度の配分
5. パレット
6. 光源の型
7. 撮影・仕上げ

---

## 1. 文学 → 光学 対照表

| 陰翳の語彙 | 画面で起きていること | 指示文に使う言葉 |
|---|---|---|
| 羊羹色／玉の温潤 | 光が表面で跳ね返らず内部に浸透し、奥からぼんやり発光する | subsurface scattering, light penetrating a few millimeters into the material, soft translucent glow from within |
| 手沢／なれ／沈んだ照り | 鏡面反射が拡散され、広く柔らかいハイライトになる | high specular roughness, micro-scratched matte patina, muted Fresnel reflection, satin sheen, worn edges |
| 光が闇から滲み出る | 光源からの距離とともに急速に暗くなり、縁だけが光を拾う | inverse-square light falloff, single practical light source, soft rim light, grazing light |
| 蝋燭・行灯の色 | 低色温度の橙色光 | 1800K–2200K blackbody color temperature, warm tungsten glow |
| 澱んだ闇 | 暗部に微かな色と情報が残っている | low-key exposure, retained shadow detail, blacks lifted slightly above pure black, rich shadow gradation, no crushed blacks |
| 障子越しの光 | 大きな拡散面が自ら発光しているように見える | large diffused backlit paper panel, self-luminous translucent surface, soft wrap light, 5000K desaturated daylight |
| 金屏風の暗がりの輝き | 暗い空間で、金属面が一点の光をかすめるように反射する | tarnished gold leaf catching a single grazing specular highlight, anisotropic metallic sheen in darkness |
| 床の間の奥の闇 | 最も奥が最も暗い、奥行き方向の光量低下 | depth falloff, background falling into near-black, atmospheric depth |
| 余白は闇 | 被写体が小さく、画面の大部分が影 | negative space filled with deep shadow, off-center subject, light-motivated vignetting |
| 見えないものの気配 | 輪郭が影に溶け、形が部分的にしか見えない | lost edges, silhouette partially dissolving into shadow, selective illumination |
| 静けさ | 動きのない構図、浅い被写界深度、長い露光感 | still life composition, shallow depth of field, calm, contemplative |

## 2. 素材別のレンダリング語

| 素材 | 指示文に使う言葉 |
|---|---|
| 黒漆 | deep black lacquer, glossy but softly diffused reflection, depth like dark liquid, faint warm undertone |
| 朱漆 | aged vermilion lacquer, worn to dark brown at the edges, satin patina |
| 金箔・金蒔絵 | tarnished gold leaf, maki-e gold dust, warm low-intensity metallic glint, anisotropic highlight |
| 素焼き・土もの | unglazed stoneware, rough porous clay surface, matte, light scattering in micro-texture |
| 灰釉・白磁 | ash-glazed ceramic, translucent porcelain rim with subsurface glow |
| 古い木 | aged hinoki / dark cedar wood, visible grain, hand-polished matte sheen |
| 和紙・障子 | washi paper fibers, translucent paper backlit, diffused glow |
| 真鍮・銅 | oxidized brass, dark bronze patina, muted metallic reflection |
| 人の肌 | skin with subsurface scattering, warm ivory tone, soft falloff, no shine |
| 絹 | dark silk with subtle woven pattern catching light at the folds |
| 液体（茶・酒） | dark liquid surface reflecting a tiny point of light, translucent amber edge |
| ガラス・プラスチック（現代物） | frosted, dulled reflections, reflections suppressed |

## 3. 刺点のレンダリング語

| 刺点 | 指示文に使う言葉 |
|---|---|
| 金の縁の一筋 | a single thin line of smoked-gold light along the rim, the only bright element in the frame |
| 湯気 | delicate wisps of steam rising, side-lit, glowing faintly against deep black, volumetric |
| 線香の煙 | a thin ribbon of incense smoke catching a narrow beam of light |
| 蝋燭の炎 | a small candle flame, slight halation, light falling off within a short radius |
| 障子の透光 | a shoji panel glowing softly from behind, the brightest surface in the room |
| 磁器・玉の透光 | a translucent porcelain rim glowing with backlight, subsurface scattering |
| 肌の透光 | light passing through the edge of the ear / fingertips, warm translucent glow |
| 液面の光 | a tiny reflection of the flame on the surface of the tea |

## 4. 明度の配分

| 領域 | 画面に占める割合 | 内容 |
|---|---|---|
| 深い闇（黒ぎりぎりで潰れない） | 40〜55% | 部屋の奥、天井、背景、呑み込まれた雑物 |
| 暗い中間調 | 25〜35% | 光の減衰域、影の中の形 |
| 仄明るい中間調 | 10〜15% | 光を受けた面 |
| ハイライト（刺点） | 1〜3% | 光源、金の縁、湯気、透光 |

- 最暗部でも RGB 8〜15 程度の色味を残す。最明部は #F0E2C0 前後にとどめ、純白にはしない。
- 刺点の周辺だけは局所コントラストを高く。画面全体は静かでも、一点ははっきりと。

## 5. パレット

| 役割 | 名前 | 目安 |
|---|---|---|
| 闇 | 黒漆 | #140F0C |
| 闇 | 墨 | #1C1A19 |
| 闇 | 煤竹色 | #2A1F17 |
| 闇 | 藍鼠 | #1E2327 |
| 闇 | 羊羹色 | #2B1A1A |
| 中間 | 飴色 | #6B4423 |
| 中間 | 焦茶 | #4A3222 |
| 中間 | 枯緑青 | #3F4A3C |
| 中間 | 錆朱 | #6E2E22 |
| 光 | 燻し金 | #A8834A |
| 光 | 蜜色 | #D9B170 |
| 光 | 象牙 | #E8D9B5 |
| 光 | 生成り（障子光） | #CFC8B8 |

境界一【残光・清寂】は墨・藍鼠・生成り・象牙が中心。境界二【金幽・絢爛】は黒漆・羊羹色・燻し金・錆朱が中心。

## 6. 光源の型

ひとつを選ぶ。混ぜない。

| 型 | 色温度 | 方向・広がり | 向く境界・題材 |
|---|---|---|---|
| 蝋燭の一灯 | 1800〜2000K | 低い位置から、狭い範囲。逆二乗で急に減衰する | 境界二。人物、器、夜の室内 |
| 燭台と金屏風 | 2000K＋金の反射 | 小さな炎を背後の金が鈍く返す | 境界二。人物、儀式的な場面 |
| 行灯 | 2200〜2500K | 和紙で拡散した柔らかな光、床に近い位置から | どちらでも。室内全般 |
| 障子越しの外光 | 4500〜5500K（低彩度） | 一方向から拡散し、奥ほど急に暗くなる | 境界一。昼の室内、和室、静物 |
| 天窓からの微光 | 5000K前後（低彩度） | 真上から細く落ちる、ごく弱い光 | 境界一。素焼きの器、ミニマルな静物 |
| 窓からの夕方の斜光 | 3000〜3500K | 低い角度で床を這う細長い光 | 現代の室内、カフェ |
| 夜の街の一灯 | 2700〜3200K | 街灯や窓の灯りひとつ、濡れた路面に長く映る | 現代の街角、路地 |

## 7. 撮影・仕上げ

- フィルム感：`Kodak Vision3 500T` または `fine 35mm film grain`。暗部にだけ見える細かい粒子。
- レンズ：`50mm or 85mm, f/1.4–2.0, shallow depth of field`。刺点にピント、周辺は柔らかく溶ける。
- ハレーション：光源の周りにごく弱い滲み（`subtle halation`）。強いグローやレンズフレアは不可。
- 表現の型：`cinematic still`, `chiaroscuro`, `low-key still life photography`。
- コントラスト：全体の明暗差は大きく、暗部の中の階調は細かく。`high dynamic range` や `HDR` とは書かない（すべてを明るく見せる処理と解釈されやすい）。
