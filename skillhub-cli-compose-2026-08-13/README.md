# SkillHub CLI + Docker Compose real-run screenshots

These assets support the bilingual SkillHub CLI and Docker Compose tutorial published on 2026-08-13.

## Files

- `01-skillhub-public-home-cn.png` — public registry homepage at `https://skill.xfyun.cn`, Chinese UI.
- `02-skillhub-public-home-en.png` — public registry homepage at `https://skill.xfyun.cn`, English UI.
- `03-skillhub-local-compose-cn.png` — self-hosted SkillHub Web UI at `http://localhost:8088`, Chinese UI.
- `04-skillhub-local-compose-en.png` — self-hosted SkillHub Web UI at `http://localhost:8088`, English UI.
- `05-skillhub-cli-real-run-cn.png` — Chinese evidence card rendered from archived output of the official `@astron-team/skillhub` CLI.
- `06-skillhub-cli-real-run-en.png` — English evidence card rendered from the same archived CLI run.

## Provenance and boundaries

- A dedicated Docker Compose project named `skillhub-t65` ran `postgres`, `redis`, `skill-scanner`, `server`, and `web`; all five containers reported healthy.
- The local Web UI returned HTTP 200 at `http://localhost:8088`; the API returned HTTP 200 with `{"status":"UP"}` at `http://localhost:18081`.
- The CLI was verified against both the public registry at `https://skill.xfyun.cn` and an explicit local registry at `http://localhost:8088`.
- The successful install shown in the CLI evidence used an authenticated public-registry session. Anonymous installation against the local registry correctly requested login.
- The local and public registries are distinct. No public-registry result is presented as a local Compose result.

Project: https://github.com/iflytek/skillhub

