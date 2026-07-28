# my-workflow-init

요구사항 문서(`requirements/`)와 진행 체크리스트(`tasks/`)를 ISO 주차(`YYYY-Www`) 폴더/파일 단위로 분리 관리하는 워크플로우를 새 프로젝트에 부트스트랩하는 [Claude Code](https://claude.com/claude-code) 스킬입니다.

## 설치

이 저장소의 내용을 프로젝트의 `.claude/skills/my-workflow-init/`에 그대로 복사(또는 서브모듈/clone)합니다.

```bash
git clone https://github.com/<your-account>/my-workflow-init.git .claude/skills/my-workflow-init
rm -rf .claude/skills/my-workflow-init/.git
```

## 사용

Claude Code 세션에서 스킬을 호출합니다 (예: "요구사항 워크플로우 세팅해줘").

세팅되는 것:
- `requirements/README.md`, `tasks/README.md` — ISO 주차 폴더/파일 관례 설명
- `docs/policies.md`, `docs/domain-model.md` — 확정 정책 / DDD 설계 스텁
- `CLAUDE.md`에 "새 요구사항 처리 절차" 섹션 추가 (문서화된 요구사항과 애드혹 요청을 구분해 처리하는 6단계 절차 + 예외 조항)

기존 파일이 있으면 덮어쓰지 않고 먼저 확인합니다. 자세한 절차는 [`SKILL.md`](./SKILL.md) 참고.
