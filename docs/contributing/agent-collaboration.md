# 에이전트 공통 협업 규칙

**협업 규칙 초안**

적용 범위는 [협업 규칙 안내](../../CONTRIBUTING.md) 참고.

Git·협업 규칙은 공유 문서를 정본으로 사용.

개인 AGENTS.md·CLAUDE.md에는 이 문서를 확인하는 지침과 도구별 활용 방식 기록.

## 문서 확인

프로젝트 진입·재개 시 이 문서와 CONTRIBUTING.md 확인.

이후 현재 작업에 필요한 구획만 확인. 같은 대화에서 매 메시지마다 전체 재독 불필요.

| 시점 | 확인할 문서 |
|---|---|
| 작업 시작·브랜치·Commit 처리 전 | [작업 흐름](workflow.md)의 브랜치·Commit 규칙 |
| Issue 작성·수정·완료 체크·종료 전 | [Issue 규칙](workflow.md#1-issue로-할-일-공유) |
| PR 작성·수정·Draft/Ready 전환 전 | [PR·검증 규칙](workflow.md#4-pr과-검증), [PR 템플릿](../../.github/pull_request_template.md) |
| 리뷰·Merge·브랜치 정리 전 | [리뷰·Merge·정리 규칙](workflow.md#5-리뷰merge정리) |
| Project 상태·Milestone·저장소 설정 변경 전 | [GitHub 운영](github-management.md)의 관련 구획 |
| 작성 예시가 필요할 때 | [작성 예시](examples.md) |

새 Issue는 목적에 맞는 템플릿 사용.

- [기능·작업](../../.github/ISSUE_TEMPLATE/task.md)
- [버그](../../.github/ISSUE_TEMPLATE/bug.md)
- [논의](../../.github/ISSUE_TEMPLATE/discussion.md)

## 작성·검증

- Git 작업 전 실제 브랜치·기존 변경 확인. PR·Merge 판단은 현재 Git·GitHub 상태 기준
- Issue·PR의 진행·완료·검증 기록은 실제 변경과 검증 근거 기준으로 작성
- 확인한 항목만 체크하고, 미검증 부분은 이유 기록
- 문서 변경은 내용·링크·예시와 기존 합의의 일관성 확인
- AI가 작성한 결과도 담당 팀원이 확인
- PR은 상대 팀원의 최종 리뷰·승인 후 Merge

## 실행 범위

질문·설명·조사·리뷰 요청은 읽기 전용으로 처리.

| 사용자 요청 | 실행 범위 |
|---|---|
| 파일 수정 | 필요한 가역적 로컬 수정과 관련 검증. commit·push·PR·merge는 별도 승인 |
| PR까지 | 필요한 commit·push·PR 작성·수정과 관련 검증. Merge 제외 |
| merge까지 | PR까지의 범위와 상대방 승인·필수 검사·리뷰 의견 처리 확인 후 Squash merge |

명시된 승인 범위 안에서는 같은 승인을 반복해서 묻지 않기.

상대방 부재 시 리뷰 대기. 파일 수정 승인을 임의로 commit·push·PR·merge 승인으로 확대하지 않기.

## 개인 안내 파일에 적용

이 파일과 기존 협업 문서는 Git으로 공유.

개인 AGENTS.md·CLAUDE.md는 각자의 Git ignore 설정으로 제외하고 관리.

각자 저장소 루트의 안내 파일에 아래 지침 추가.

```markdown
## 공통 협업 규칙

- 프로젝트 진입·재개 시 docs/contributing/agent-collaboration.md 확인
- 현재 작업에 해당하는 공통 규칙·템플릿을 확인하고, 합의된 규칙 준수
```

공통 기준 변경은 공유 문서에 반영. 파일 경로가 바뀌면 각자의 안내 파일도 갱신.
