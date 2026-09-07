# Receiver Confirmation

このCTXを受け取って作業を再開してください。

**今回進めたい作業：**
[ここに、いま再開したい案件・作業を1行で書いてください]

ただし、**内容が正しいCTXであることと、今再開すべきCTXであることは別です。**
作業や外部変更を始める前に、上の「今回進めたい作業」とCTXの再開識別情報が一致しているか確認してください。

開始前に、あなたが理解した内容を次の9項目で返してください。

1. WORK ID／ACTIVE WORKSTREAM
2. CURRENT OBJECTIVE／OBJECTIVE KEY
3. PARENT WORK／RELATED・SIDE WORK
4. 現在地
5. 決定事項
6. 保留事項（ブロックの有無を含む）
7. 制約・注意点
8. 次にやること
9. RESUME ENTRY判定：`PASS` / `CONFIRM_REQUIRED` / `BLOCK` / `SWITCH_REQUIRED`

判定の意味：

- `PASS`：今回進めたい作業と、このCTXのworkstream・目的・親作業が一致している。
- `CONFIRM_REQUIRED`：今回進めたい作業が示されていない、識別情報が不足している、複数候補がある、またはどれを再開するか確定できない。
- `BLOCK`：有効なCTXではあるが、今回進めたい作業とは別のworkstream／目的を指している。
- `SWITCH_REQUIRED`：別workstreamへ切り替える意思は確認できるが、現在のActive Workとの切替確認が必要。

**`PASS`の場合だけ**「次にやること」の1番へ進んでください。

`CONFIRM_REQUIRED`、`BLOCK`、`SWITCH_REQUIRED`の場合は作業を進めず、不一致・不足している項目を具体的に示してください。Git/GitHubへの書き込み、公開、削除、外部送信などの状態変更も行わないでください。

CTXに書かれていない情報は、推測で補わないでください。
