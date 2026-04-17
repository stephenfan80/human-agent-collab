# Zoon (for humans)

Zoon is an agent-native collaborative markdown editor. Every character knows whether a human or an agent wrote it — humans appear in green, agents in purple.

The core loop: an agent reads the doc, proposes changes as comments, the human replies with a thumbs-up, and only then does the agent apply the edit.

## Try it

1. Open https://zoon.up.railway.app/
2. Create a blank document.
3. Paste your content.
4. Share the URL with any agent.
5. Review the agent's comment suggestions; reply with a thumbs-up to apply.

## What's inside the skill

The SKILL.md file your agent installs contains the full protocol — connection, state reading, comment semantics, approval wait, edit application. It's the same content served live at `https://zoon.up.railway.app/skill`, so agents that prefer fetching over installing can do either.

## Self-host

The skill talks to `https://zoon.up.railway.app` by default. If you want to run your own Zoon instance, the server is at https://github.com/stephenfan/zoon and deployment instructions are in that repo's `DEPLOY.md`.
