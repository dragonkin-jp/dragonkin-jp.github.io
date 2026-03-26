# パッチノート

> 📌 情報源: aRPG Timeline / Steam / Nacon公式 / SteamDB / GameHelper.io（2026年3月更新）
アップデート情報を時系列でまとめるページ。

---

## v1.3.66.54113 — 第2ポストローンチホットフィックス（2026年3月下旬）

### クエスト・進行バグ修正
- 「**Talk to the Grand Tracker Yula**」完了後、都市から平原へのテレポーターがミニマップに表示されないバグを修正
- クエスト「**The Battle of Pont-Noir**」で進行不能になるブロッカーを修正
- クエスト「**Blood Sorcery**」でレーザーが特定角度でスタックして進行不能になるブロッカーを修正（第1ホットフィックスの「Execution系スキルでの進行不能」とは別バグ）
- ストーリー**最終幕でチャンピオンが複数スポーンまたはゼロスポーンになる**進行ブロッカーを修正

### グラフィック・UI
- 同モデルのモニターを複数接続している場合に設定画面に表示されないバグを修正
- **RTX 40/50系GPUでブラックスクリーンクラッシュが発生する問題**：Frame Generation と Reflex の競合が原因と特定。暫定対処としてFrame Genを無効化（恒久修正は次パッチ予定）

### 未修正の既知バグ（この時点）
- **ルートフィルター停止問題**：起動後一定時間でフィルターが機能しなくなる不具合。暫定回避策はゲームの再起動

---

## v1.0 ポストローンチ ホットフィックス（2026年3月）

### クエスト・進行バグ修正
- エンドゲームクエスト **7-4**「The Monster of Erde-nòr」がスポーンせず進行不能になるバグを修正
- クエスト「**Blood Sorcery**」でExecution系スキルを使ってシャーマンを倒すと次に進めなくなるバグを修正

### クラス・タレント・スキル修正
- トラッカータレント「**Mounted Hunt**」で2つの移動スキルを連続使用すると半騎乗状態のまま固まるバグを修正
- トラッカータレント「**Pack Hunter**」がグランドベネディクター（Grand Benedictor）で全クラスに表示されるバグを修正（トラッカー専用）。また、戦闘中に装備するとゲームがクラッシュするバグも修正
- クラス専用モディファイアが他クラスの非対応スキルにも適用されクラッシュするバグを修正
- 「**Limitless**」モディファイアが以下に正しく適用されるよう修正: Pale Dragon's Aura / Cobalt Dragon's Aura / Toxic Spray
- Oracleスキル「**Pythoderkon's Premonition**」にクールダウンタグが表示されないバグを修正

### 通信・安定性
- クラッシュの修正（複数）
- オンライン接続不具合の修正（Mynakonサーバーとの接続問題）

> ⚠️ オンラインセッションへの参加にはゲームの最新バージョンへのアップデートが必要。問題が続く場合は公式Discordへの報告を推奨。

### 未修正の既知バグ（2026年3月時点）
以下のバグはこのホットフィックスでは**修正されていない**。引き続き公式パッチを待つ状況：
- **「The Lost Scale」クエスト — Son-Kan NPC消失**：NPCが会話途中で消え進行不能になる。コミュニティ回避策あり（[multiplayer.md 参照](../multiplayer.md)）
- **マルチプレイ キャラクター進行問題**：ゲストとして参加した場合、キャラクターがホストワールドにリセットされる仕様
- **敵スケーリング問題**：Co-op時に敵がパーティ最高レベルに合わせてスケールする

[Steam: Hotfix now live](https://store.steampowered.com/news/app/1863430/view/532124583945306657)

---

## v1.0.0 — 正式リリース（2026年3月16日）

### 主な追加・変更内容
- ストーリー Act 2・3・4 を追加（全4幕が揃い完結）
- ローカルCo-op（カウチCo-op）を最大2人で実装
- アンセストラルグリッドに新タレント×8追加
- Steamアチーブメント **44個** を実装
- 無料コスメティックDLC「**Light of the First Praise**」配布（Discord経由、期間限定）
- Twitch Dropsキャンペーン（〜2026年3月31日）
- PS5・Xbox Series X|S版リリース: 3月19日

### バランス・経済変更
- プリモーディアル・ダスト（Primordial Dust）のリロールコスト **−60%**
- 素材の所持上限を **99,999** まで拡張
- ゴールド・経験値の獲得量を全体的に **+30%** 増加

[  詳細: aRPG Timeline](https://www.arpg-timeline.com/game/dragonkin-the-banished)
[  v1.0リリース記事 (Soren.com)](https://soren.com/en/news/dragonkin-the-banished/2026-03-16-dragonkin-the-banished-10-unleashes-full-story)

---

## v0.9 — マルチプレイアップデート（2026年2月25日）

Early Access最後の大型アップデート。オンラインCo-opを正式実装。

### 主な追加・変更内容
- **オンラインCo-op（最大4人）** を実装
- モンテスカイルの進行システムを刷新（よりシンプルかつ明確な構成に）
- スキルとエネルギーコストを全面改訂（Generator/Spenderシステムを廃止）
- 各クラスに新タレントを追加（詳細は [ancestral-grid.md](../ancestral-grid.md) 参照）
- Lv.50以降の進行（アンセスターEXP）を正式導入

### バグ修正
- Catacombs of Fire・Plains of Koles・Fafnir's Glacierで透明な壁によりプレイヤーが進行不能になるバグを修正
- エンドゲームまたは既存ストーリーグループで新キャラクターを開始した際のデフォルトスキル・装備が正しく設定されないバグを修正
- クエストダイアログを素早くスキップした際に報酬が空になるバグを修正
- ワイバーミングのアトリビュートポイントを再振り分けした際にタレントがリセットされるバグを修正

[Steam: Multiplayer Patch Notes!](https://store.steampowered.com/news/app/1863430/view/576019638373057668)
[SteamDB: マルチプレイパッチノート詳細](https://steamdb.info/patchnotes/22002239/)

---

## Early Access 期間（2025年3月6日〜2026年3月15日）
約1年のEarly Access期間中、コミュニティのフィードバックを元に継続的にアップデートが行われた。
- Act 1（ジャングルバイオーム）のみプレイ可能だった
- アンセストラルグリッドシステムを段階的に改良
- バランス調整・バグ修正を多数実施

---

## 情報源
[aRPG Timeline - アップデート一覧](https://www.arpg-timeline.com/game/dragonkin-the-banished)
[Steam コミュニティ（パッチノート）](https://steamcommunity.com/app/1863430)

---
