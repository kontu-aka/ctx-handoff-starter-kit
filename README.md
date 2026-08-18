# CTX Handoff Starter Kit v0.1

AIとの長い作業を、**新しいチャットや別のAIへ引き継ぐ**ための無料公開版スターターキットです。

前回の「決定したこと」「保留していること」「却下したこと」「次にやること」を1枚のCTXにまとめ、
受け取ったAIに理解内容を確認させてから作業を再開します。

## こんな方へ

- ChatGPT・Claude・Gemini・Codex・Claude Code などを複数使い分けている
- ひとつの作業が数日以上またぐことがある
- 新しいチャットを開くたびに、前回の経緯を説明し直している
- 「これ決めたはずなのに」「これは却下したはずなのに」が起きたことがある

## まず試す

1. [`examples/SAMPLE_KURUMIDO.md`](examples/SAMPLE_KURUMIDO.md) の記入済みCTXを見る
2. CTX部分をコピーして、新しいチャットまたは別のAIへ貼る
3. [`templates/RECEIVER_CONFIRMATION_MIN.md`](templates/RECEIVER_CONFIRMATION_MIN.md) の受領確認文を続けて貼る
4. AIが現在地・決定・保留・制約・次の一手を理解できているか確認する
5. 自分の作業では [`templates/CTX_HANDOFF_MIN_TEMPLATE.md`](templates/CTX_HANDOFF_MIN_TEMPLATE.md) を埋める

## 何を揃えるのか

CTXでは、会話全部を保存するのではなく、**続きから再開するために必要な状態**を残します。

- 目的
- 現在地
- 決定事項
- 保留事項
- 却下事項
- 作成・変更ファイル
- 制約・保存上の注意
- 次にやること
- 未確認事項

## 3つのAIでの実測

2026-08-16 に、同じサンプルCTXを ChatGPT・Claude・Gemini に渡して確認しました。

| 確認項目 | ChatGPT | Claude | Gemini |
|---|:---:|:---:|:---:|
| 復唱してから作業を始めたか | ✕ | ○ | ○ |
| 決定事項を維持したか | ○ | ○ | ○ |
| 却下済み案を復活させなかったか | ○ | ○ | ○ |
| 未提示情報を捏造しなかったか | ○ | ○ | △ |
| 指示された次作業を実行したか | ○ | ○ | ○ |

CTXの目的は**すべてのAIに同じ答えを出させることではありません**。
AIごとの考え方や表現は違っても、作業の土台となる決定・保留・却下・制約・次の一手を持ち運びやすくすることが目的です。

詳しくは [`examples/SAMPLE_KURUMIDO.md`](examples/SAMPLE_KURUMIDO.md) をご覧ください。

## 使い方のコツ

**作業を終えるときに書く。** 再開するときではなく、記憶が残っているうちに残します。

**全部書こうとしない。** 会話の再現ではなく、続きから始められる状態を渡すことが目的です。

**未確認は未確認と書く。** 空欄にせず、「未提示。推測しないこと」と明示します。

## 注意

- 本セットはテンプレートと手順です。ソフトウェアやアプリではありません。
- AIの応答内容・記憶・精度を保証するものではありません。
- **パスワード、APIキー、認証情報、個人情報、顧客の秘密情報はCTXに書かないでください。**
- チーム向けの権限管理・監査ログ・共有Control Planeなどは、この無料公開版には含まれません。

## ファイル

- [`templates/CTX_HANDOFF_MIN_TEMPLATE.md`](templates/CTX_HANDOFF_MIN_TEMPLATE.md) — 記入用テンプレート
- [`templates/RECEIVER_CONFIRMATION_MIN.md`](templates/RECEIVER_CONFIRMATION_MIN.md) — 受領AIへの確認文
- [`examples/SAMPLE_KURUMIDO.md`](examples/SAMPLE_KURUMIDO.md) — 記入例＋3AI実測
- [`FAQ.md`](FAQ.md) — よくある質問
- [`TERMS.md`](TERMS.md) — 利用条件

## ライセンスについて

本配布物は無料公開版ですが、再配布・再販売を許可していないため**オープンソース（OSS）ではありません**。
詳しくは [`TERMS.md`](TERMS.md) をご確認ください。

---

v0.1 / 2026-08-16
