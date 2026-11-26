# 보안점검딸깍

바이브 코딩으로 만든 웹 서비스(Next.js, Vercel, Supabase, AI API)를 **쉬운 말로 보안 점검**하는 Codex, Claude Code용 스킬입니다.
비밀 키, 화면과 서버, 로그인과 권한, Supabase RLS와 정책, 파일 보관함, AI 비용, 개인정보를 확인하고 **꼭 고칠 3개**를 골라 줍니다.
점검만 하고 코드는 바꾸지 않습니다. `.env` 파일은 열지 않습니다.

## 설치

프로젝트 폴더에서 터미널을 열고 한 줄이면 됩니다.

```bash
npx skills add AIjunja/vibe-security-check --skill 보안점검딸깍
```

또는 Codex에게 이렇게 말하세요.

```text
https://github.com/AIjunja/vibe-security-check 의 skills/보안점검딸깍 폴더를
지금 프로젝트의 .agents/skills/보안점검딸깍 으로 받아 줘.
받은 뒤 /skills 목록에 보이는지 확인해 줘.
```

## 쓰는 법

| 도구 | 부르는 방법 |
| --- | --- |
| Codex | `$보안점검딸깍 내 서비스 점검해 줘` |
| Claude Code | `/보안점검딸깍 내 서비스 점검해 줘` |

결과에서 고칠 번호를 골라 "1번, 3번만 고쳐 줘"라고 말하면 그것만 고칩니다.

## 더 깊게 보고 싶다면

- Cloudflare 공식 security-audit 스킬: `npx skills add https://github.com/cloudflare/security-audit-skill --skill security-audit`
- 남이 만든 스킬이나 레포가 걱정되면 설치 전에 SKILL.md와 AGENTS.md를 먼저 읽고, [NVIDIA SkillSpector](https://github.com/NVIDIA/skillspector)로 검사하세요.

## 출처와 주의

- 테이텀 시큐리티(@tatum_hq)의 「바이브코더를 위한 실전 보안 가이드」를 Threads @reviewdap.ai가 재구성한 점검 프롬프트를 바탕으로, 수업용으로 범위를 줄이고 쉬운 말로 고쳤습니다.
- 이 점검은 백신이 아닙니다. 통과해도 완전히 안전하다는 뜻은 아닙니다. 법률 자문이 아닙니다.
