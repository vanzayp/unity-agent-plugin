# Unity Agent Plugin — Skills 日本語訳

このファイルは `skills/` 配下のSkillについて、AIが何をするための機能なのかを日本語で確認するための一覧です。Skill名・Unity API名・パッケージ名・コマンド名は原文どおり保持します。

## 2D / グラフィックス

### `2d-pixel-perfect` — 2Dピクセルパーフェクト
Pixel Perfect Cameraを使用する2Dゲーム向けに、解像度・ピクセル比・カメラ設定などを調整し、スプライトが意図したピクセル単位の表示になるよう設定・確認するためのSkillです。

### `audio-setup-mixers` — Audio Mixerのセットアップ
Unity Audio Mixerを作成・設定し、Audio Mixer Group、音量制御、エフェクト、ルーティングなどを構成するためのSkillです。

### `build-live-game` — ライブゲームを構築
Unity Gaming Services (UGS) を利用したライブサービス機能を構築・接続・デバッグするためのSkillです。Authentication、Cloud Code、Cloud Save、Remote Config、Deployment、Economy、Leaderboards、Achievements、Battle Pass、Player Accountなどを扱います。ゲームの整合性に関係するXP・報酬・通貨などはCloud Code側で処理することを重視します。

### `generate-editor-search-query` — Unity Editor検索クエリ生成
Unity Editor内の検索に使用する検索クエリを生成するためのSkillです。対象アセットやGameObjectなどを検索する際に、Unityの検索構文に合わせたクエリを組み立てます。

### `implement-in-app-purchases` — アプリ内課金を実装
Unity IAPを使用して商品、購入処理、購入確認、復元、ストア設定などを実装するためのSkillです。

### `initialize-ai-navigation` — AI Navigationを初期設定
Unity AI NavigationのNavMeshSurface、NavMeshAgent、NavMeshObstacle、NavMeshLink、NavMeshModifier、Area、Costなどを設定します。歩行可能領域のBake、経路探索、障害物回避、Patrol、Click-to-Move、Animatorとの連携なども対象です。

### `levelplay-unity-integration` — LevelPlayをUnityへ統合
UnityプロジェクトへLevelPlay広告SDKを導入し、広告フォーマット、初期化、広告表示、報酬付き広告などを設定・統合するためのSkillです。

### `localization` — ローカライズ
Unity Localizationを使用した多言語対応を設定します。String Table、Asset Table、Locale、ローカライズされたアセットや文字列の参照・切り替えなどを扱います。

### `manage-sprite-atlas` — Sprite Atlasを管理
Unity Sprite Atlasの作成・設定・パック対象の管理・テクスチャ圧縮など、SpriteをAtlasへまとめるための操作を扱います。

### `migrate-birp-to-urp` — Built-in Render PipelineからURPへ移行
Built-in Render Pipeline (BiRP) のプロジェクトをUniversal Render Pipeline (URP)へ移行する際の設定、マテリアル、シェーダー、レンダリング設定などを整理・変換するためのSkillです。

### `new-unity-project` — 新規Unityプロジェクト作成
Unityプロジェクトを新規作成し、必要なテンプレート・設定・パッケージなどを初期化するためのSkillです。

### `optimize-audio` — オーディオを最適化
UnityのAudioClip、Import Settings、圧縮形式、Load Type、Preload Audio Dataなどを確認し、メモリ使用量、ロード時間、再生性能などを改善するためのSkillです。

### `optimize-text-mesh-pro` — TextMeshProを最適化
TextMeshProのFont Asset、Dynamic Atlas、Fallback、Padding、Sampling、SDF16、AutoSize、UGUI / World Space、CJKフォントなどを対象に、表示品質・メモリ・CPU性能・多言語対応を最適化します。

### `optimize-web` — Web向けUnityを最適化
Web向けビルド、とくにWebGL系のロード時間、メモリ、ビルドサイズ、ランタイム性能などを改善するためのSkillです。

### `physics-3d-collision` — 3D物理衝突を設定
Collider、Rigidbody、Physics Layer、Physic Material、TriggerなどUnityの3D物理衝突を設定・診断するためのSkillです。

### `setup-multiplayer-services` — Multiplayer Servicesをセットアップ
Unity Multiplayer Servicesを使用したマルチプレイヤー機能を設定します。セッション、接続、ロビーなど、Unityのマルチプレイヤー関連サービスをプロジェクトへ導入するためのSkillです。

### `setup-vivox-voice-chat` — Vivoxボイスチャットをセットアップ
VivoxをUnityプロジェクトへ統合し、音声チャンネルへの参加、プレイヤーの接続、音声通信などのボイスチャット機能を構築するためのSkillです。

### `shader-graph-create-custom-node` — Shader Graphカスタムノードを作成
Shader Graphで利用できるCustom Function / Custom Node系の処理を作成し、独自のシェーダー処理をShader Graphへ組み込むためのSkillです。

### `sprite-editor` — Sprite Editorを操作
`ISpriteEditorDataProvider` APIを使用して、SpriteのRect、Border、Pivot、Outline、SliceなどのSpriteメタデータをEditor上で変更します。Automatic / Grid / IsometricのSliceにも対応します。`.meta`を直接編集するのではなく、ImporterのAPIを使用します。

### `sprite-segment-3x3grid` — Spriteを3×3グリッドへ分割
Spriteを9スライス用の3×3領域へ分割・設定するためのSkillです。UIなどで中央を伸縮させつつ端を維持する用途を想定します。

### `tilemap-palette-create` — Tilemap Paletteを作成
Unity Tilemapで使用するTile Paletteを作成・構成し、TileアセットをPaletteへ登録してレベル制作で利用できる状態にするためのSkillです。

### `tilemap-ruletile-createempty` — 空のRule Tileを作成
Tilemap用のRule Tileを新規作成し、隣接Tileの条件に応じて表示Tileを切り替えるための基本設定を作るSkillです。

### `tilemap-ruletile-createfromsegment` — セグメントからRule Tileを作成
Spriteのセグメント情報などを利用して、Tilemap用Rule Tileを生成・設定するためのSkillです。

## UI

### `ui-imgui` — IMGUI UIを作成・操作
Unity Editorで使用するIMGUIベースのカスタムUIを作成します。EditorWindow、Inspector、GUILayout / EditorGUILayoutなどを使用したEditor拡張を対象とします。

### `ui-ugui` — uGUIを構築
Canvas、RectTransform、Image、Text / TextMeshPro、Button、Layout Groupなど、UnityのuGUIを使用したランタイムUIを構築・設定するためのSkillです。

### `ui-uitk` — UI Toolkitを構築
UI Toolkitを使用してVisualElement、UIDocument、UXML、USSなどからUnity UIを構築します。ランタイムUIとEditor UIの両方を対象にします。

### `ui` — Unity UI全般
Unity UIに関する要求を判断し、uGUI、UI Toolkit、Editor UIなど適切なUI技術を選択・構築するための包括的なSkillです。

## Unity環境・パッケージ

### `unity-cli` — Unity CLI / Editor連携
Unity CLIを導入・確認し、接続されたUnity Editorの状態や利用可能なコマンドを確認して、AIエージェントからEditorを操作するための基盤Skillです。`unity command`、Editorへの接続確認、コマンドカタログの取得などを扱います。

### `unity-package-management` — Unity Package管理
`Packages/manifest.json`、Unity Package Manager、Registry Package、Git Packageなどを扱い、Unityパッケージの追加・更新・削除・確認を行うためのSkillです。

## URP

### `urp-postprocessing` — URPポストプロセスを設定
URPで使用するVolume、Post-processing効果、Renderer Featureなどを設定し、画面全体のポストプロセスを構成するためのSkillです。

### `validate-urp-render-graph-renderer-feature` — URP Render Graph Renderer Featureを検証
URPのRender Graph対応Renderer Featureについて、Render Pass、ResourceHandle、Context、ライフサイクルなどの使い方を確認し、Render Graph上で問題が起きる実装を検証・修正するためのSkillです。

## 注意

このファイルは「機能の日本語訳・索引」です。元の `SKILL.md` に含まれるコード、API仕様、詳細な手順、参照ドキュメントまで逐語翻訳したものではありません。元Skillそのものを日本語化する場合は、各 `SKILL.md` の本文を維持したまま英語の説明文を日本語へ置換し、コード・API名・パッケージ名・ファイルパス・コマンドを変更しない形にする必要があります。
