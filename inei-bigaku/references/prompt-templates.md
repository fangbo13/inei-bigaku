# プロンプト雛形

`{ }` を観察の結果で埋める。英語本文は画像モデル用、日本語要約はユーザー確認用。

**書き方の原則**
- 詩的な形容詞を並べない。**光源の種類・位置・色温度／何が光を拾うか／何を闇に呑ませるか／素材の反射特性** を、`optics-and-palette.md` の光学の言葉で書く。
- 刺点は「画面で最も明るい要素」として明記する。書かないと、モデルは全体を均一に暗くする。
- 引き算ははっきり命令する。「背景を暗く」ではなく「other cups are swallowed by darkness / cropped out」と書く。

## 目次
1. Gemini：境界一【残光・清寂】
2. Gemini：境界二【金幽・絢爛】
3. Gemini：現代都市・夜
4. Gemini：主題を保つ場合（人物・「構図はそのまま」の指定）
5. 修正の指示
6. Midjourney
7. Stable Diffusion / Flux（img2img）

---

## 1. Gemini：境界一【残光・清寂】

```
Re-photograph this scene as a quiet, minimalist low-key still life in the aesthetic of Tanizaki's "In Praise of Shadows".

Composition (subtractive): keep only {the single anchor, e.g. "the unglazed teapot"} as the subject. {Crop in closely / reframe} so it sits slightly off-center. {Everything else, e.g. "the other five cups, the tray and the table edge"} is swallowed by deep shadow or cropped out of frame. Most of the frame is negative space filled with darkness.

Light: a single weak, cool, desaturated daylight source (about 5000K), falling as a narrow beam from {direction, e.g. "a high window on the upper left"}, diffused as if through shoji paper. Strict inverse-square falloff: the light dies within a short distance. No other light in the scene.

Visual anchor (the brightest element in the frame): {punctum, e.g. "delicate wisps of steam rising from the spout, side-lit, glowing faintly white against the black background"}.

Materials: {e.g. "rough unglazed stoneware"} with high specular roughness and a matte, hand-worn patina; ash-glazed rims show a faint subsurface glow. Washi-like softness in the light.

Tone: low-key exposure with retained shadow detail; blacks lifted just above pure black, in ink-grey and indigo-grey gradations. Highlights small and soft, ivory, never pure white. Low saturation.

Camera: 50mm, f/2, shallow depth of field, focus on the anchor; fine 35mm film grain in the shadows.

Mood: solitary, silent, contemplative wabi-sabi stillness; much is left unseen for the viewer to imagine.
Do not add any objects, props, or Japanese decorations that are not in the photo (light, steam and smoke are allowed).
Avoid: horror, gothic, film-noir hard shadows, HDR, oversharpening, a flat underexposed look, a mechanical vignette.
```
**日本語要約**：{アンカー}だけを残して寄りで切り取り、ほかは闇へ。天窓・障子越しの冷たく弱い一灯。刺点は{刺点}。墨と藍鼠の階調、素焼きの艶消し。侘びの静けさ。

## 2. Gemini：境界二【金幽・絢爛】

```
Re-photograph this scene as a deep, luxurious low-key image in the aesthetic of Tanizaki's "In Praise of Shadows" — black lacquer and faint gold in candlelight.

Composition (subtractive): keep only {anchor} as the subject, {crop / reframe}. {Everything else} dissolves into lacquer-black darkness or is cropped out. Lost edges: the far side of the subject melts into shadow.

Light: a single candle flame (1800K blackbody color) placed low at {position}, the only light source. Inverse-square falloff: warm light within a small radius, deep darkness beyond it. A faint warm rim light on the subject's edge.

Visual anchor (the brightest element in the frame): {punctum, e.g. "a single thin line of tarnished gold along the rim of the lid, catching a grazing specular highlight"}.

Materials: {e.g. "the surfaces rendered as black lacquer with a softly diffused, liquid-deep reflection; details in tarnished maki-e gold"}; high specular roughness, muted Fresnel reflection, satin patina — no new gloss. Where light passes through thin or translucent parts, subsurface scattering gives a dim inner glow.

Tone: 75% of the frame in deep shadow with rich gradation of lacquer-black, dark azuki-red and soot-brown; blacks never crushed. Highlights small, honey and smoked-gold, never white. Low saturation except the gold.

Camera: 85mm, f/1.8, shallow depth of field; subtle halation around the flame; Kodak Vision3 500T grain.

Mood: profound, dignified, hushed, ceremonial; a single breath of light inside an endless darkness.
Do not add props, costumes, or Japanese decorations not present in the photo (light, candle glow, steam and smoke are allowed).
Avoid: horror, gothic, film-noir hard shadows, HDR, glossy CGI, oversaturated orange, a flat underexposed look.
```
**日本語要約**：{アンカー}だけを残し、黒漆の闇へ。低い位置の蝋燭一灯（1800K）。刺点は{刺点}。燻し金と羊羹色、沈んだ照り。深遠な気品。

> 蝋燭を「画面に描き込む」かどうか：元写真に蝋燭がなければ、光源は画面外に置く（`an off-screen candle`）。画面内に炎を足すのは再解釈として強く寄せるときだけ。

## 3. Gemini：現代都市・夜

```
Re-photograph this scene as a cinematic still in the aesthetic of Tanizaki's "In Praise of Shadows", transposed to the modern city.

Composition (subtractive): keep {anchor, e.g. "the lone figure at the counter" / "one lit window" / "the coffee cup and the hand"}. The rest of the scene — {signs, crowds, clutter} — dissolves into deep shadow; any text or logos become unreadable.

Light: all ceiling lights, fluorescent tubes and neon are switched off. The only light is a single warm tungsten practical (about 2800K) {e.g. "a small table lamp" / "one streetlamp" / "a window across the alley"}. Inverse-square falloff; soft rim light on the anchor.
{If outdoors: "Rain-wet pavement reflects the single light in a long, soft streak."}

Visual anchor (the brightest element): {punctum, e.g. "steam curling from the cup, catching the lamp light"}.

Materials: glass, metal and plastic lose their sharp reflections — frosted, dulled, high specular roughness.

Tone and color: low-key chiaroscuro with retained shadow detail; deep green and brown shadows; desaturated; lighting inspired by Christopher Doyle's work in "In the Mood for Love", but without neon or saturated red/green.

Camera: 35mm or 50mm, f/1.8; Kodak Vision3 500T, fine grain, subtle halation.

Mood: quiet urban solitude; stillness; most of the city is left to the imagination.
Do not add Japanese props or decorations.
Avoid: neon, cyberpunk, harsh contrast, HDR, cold blue tint, a flat underexposed look.
```
**日本語要約**：照明を消して一灯のタングステン光だけに。{アンカー}と{刺点}以外は闇へ。文字は読めなくする。深緑と焦茶の影、濡れた反射、低彩度。

## 4. Gemini：主題を保つ場合（人物・「構図はそのまま」の指定）

1〜3のどれかの雛形の Composition を、次に差し替える。

```
Composition: keep the original framing, and keep {the person's face, features, expression and age} exactly the same.
Subtraction happens only through light: {background, clothing, other people and objects} sink into deep shadow so they are barely sensed.
```
人物の刺点の例：`warm translucent glow at the edge of the ear and fingertips (subsurface scattering)`、`a single small catchlight in one eye`

## 5. 修正の指示（2回目以降）

| 症状 | 追加指示 |
|---|---|
| ただの露出不足に見える | `This looks merely underexposed. Make {punctum} clearly the brightest element with strong local contrast, and add more tonal gradation inside the shadows.` |
| 雑物が残っている | `Crop closer to {anchor}. Let {remaining clutter} disappear completely into darkness.` |
| 暗すぎて主題が消えた | `Lift the light on {anchor} slightly so it is clearly readable; keep everything else as it is.` |
| 光がぎらつく | `Increase specular roughness: highlights smaller, softer and warmer, like candlelight on old lacquer.` |
| ホラーっぽい | `Make the mood calm and tender, not eerie; warm the shadows toward brown and amber.` |
| オレンジ一色になった | `Reduce saturation; keep the warmth only near the light source and let the shadows go to neutral lacquer-black.` |
| 和の小道具が足された | `Remove the added {props}; keep only what was in the original photo.` |

## 6. Midjourney

```
{image URL} {anchor in a short phrase}, in the aesthetic of Tanizaki's In Praise of Shadows, {register: "wabi-sabi, unglazed stoneware, faint cool skylight" / "black lacquer and tarnished gold, single 1800K candle"}, inverse-square light falloff, {punctum}, everything else swallowed by darkness, negative space, high specular roughness matte patina, subsurface scattering, low-key with retained shadow detail, Kodak Vision3 500T, fine grain, quiet meditative stillness --iw 1.0 --style raw --s 150 --ar {ratio} --no horror, neon, HDR, harsh contrast, pure white highlights, clutter
```
- 構図を保つなら `--iw 1.5〜2.0`、引き算で大きく変えるなら `0.5〜1.0`。

## 7. Stable Diffusion / Flux（img2img）

**Positive**
```
in praise of shadows aesthetic, low-key still life, {anchor} only, {punctum}, single {light source} {color temperature}, inverse-square falloff, soft rim light, negative space filled with deep shadow, retained shadow detail, high specular roughness, matte patina, subsurface scattering, {register materials}, low saturation, Kodak Vision3 500T, fine film grain, quiet, contemplative
```
**Negative**
```
horror, gothic, film noir, hard shadows, HDR, oversharpened, neon, blue tint, pure white, blown highlights, specular glare, glossy CGI, plastic, clutter, many objects, flat underexposed, tourist japanese props, kimono, torii, cherry blossoms
```
- Denoising strength：主題保持 0.35〜0.5、引き算・再構成 0.55〜0.7
- 構図を保つなら ControlNet（Depth/Canny）を併用。引き算でクロップするなら、先に画像を切り取ってから img2img にかける。
