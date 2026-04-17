# human-agent-collab · 人和 Agent 协作 skill

Drop-in skill: any agent can collaborate on a shared markdown document with a human via plain HTTP. Agents propose edits as comments; nothing lands without a 👍 from the human. No SDK, no browser automation, no special libraries — just HTTP + JSON.

即插即用的 skill：任何 agent 都能通过纯 HTTP 协议和人类在一份共享 markdown 文档里协作。Agent 以评论形式提出修改，人回复 👍 才落地。

## For your agent (one command)

**Claude Code:**
```
/plugin marketplace add stephenfan80/human-agent-collab
/plugin install zoon@human-agent-collab
```

**Codex / any HTTP-capable agent:**

Share either URL with your agent and tell it to follow the instructions. Prefer the live endpoint — it always matches the deployed service:

- Live: `https://zoon.up.railway.app/skill`
- Pinned copy (synced from the live endpoint): `https://raw.githubusercontent.com/stephenfan80/human-agent-collab/main/SKILL.md`

## What the agent does

1. You share a doc URL.
2. The agent reads the doc.
3. The agent proposes edits as comments.
4. You reply with a 👍.
5. The agent applies the edit.

No edit lands without your approval.

## Humans: how does this work?

See [`docs/human.md`](docs/human.md).

## License

MIT.
