
[VSCode v1.99](https://code.visualstudio.com/updates/v1_99) よりGitHub Copilot ChatのエージェントモードがGAになった

有効化するためには、settings.json 有効化の設定を追加する

```json:settings.json
{
  "chat.agent.enabled": true,
}
```

自分が使えたモデルは以下

- Claude 3.5 sonnet
- Claude 3.7 sonnet
- GPT-4o

基本的にはClaude 3.7 sonnetを使っている

- MCPのサポートが追加されている
- プロンプトで、`#fetch` にURLを追加することで、そのURLページ内の情報を取得して思考する機能の追加
- `Thinking tool`
- `#usages` で `"Find All References", "Find Implementation", and "Go to Definition"` を明示的に指定できる
  - Agent モードでは明示せずとも良い
