# DevOps · 코딩 규칙 인덱스 (FridgeAI)

> **Cursor / Agent 진입점**  
> `backend/.cursorrules` 또는 `.cursor/rules/*.mdc` 를 읽은 뒤, **반드시 본 파일과 작업 영역에 맞는 하위 문서**를 확인하고 코드를 작성한다.

---

## 필수 읽기 순서

| 순서 | 문서 | 용도 |
|------|------|------|
| 1 | [`backend/.cursorrules`](../../backend/.cursorrules) | 하네스·검증·자율성 경계 |
| 2 | [`backend/CLAUDE.md`](../../backend/CLAUDE.md) | 구현 전 사고, 단순성, 정밀 수정 |
| 3 | **본 파일** (`docs/DevOps/README.md`) | 영역별 규칙 목록 |
| 4 | 아래 표에서 **해당 영역** 문서 | 구체적 코딩 규칙 |

---

## 영역별 규칙

| 영역 | 문서 | 적용 경로 |
|------|------|-----------|
| **Backend (FastAPI)** | [Backend/BACKEND_RULES.md](./Backend/BACKEND_RULES.md) | `backend/**` |
| **Backend (DB·엔티티)** | [Backend/ENTITY_RULE.md](./Backend/ENTITY_RULE.md) | `backend/**/models/**`, Alembic |
| **Frontend (React)** | [Frontend/REACT_RULES.md](./Frontend/REACT_RULES.md) | `frontend/**` |

---

## 도메인 · 프로젝트 문서 (`docs/`)

| 주제 | 경로 |
|------|------|
| FridgeAI 기획·에이전트 | [`docs/프리지개발/`](../프리지개발/) |
| UI | [`docs/프리지개발/260506_fridge_UI.md`](../프리지개발/260506_fridge_UI.md) |
| FastAPI 실행 메모 | [`docs/수업 메모/FastAPI + Unicorn 설치 & 실행.md`](../수업%20메모/FastAPI%20+%20Unicorn%20설치%20&%20실행.md) |
| 디자인 패턴 | [`docs/수업 메모/디자인패턴.md`](../수업%20메모/디자인패턴.md) |

---

## 규칙 추가·변경

- 반복되는 지시는 **해당 `docs/DevOps/{Backend|Frontend}/` MD**에 추가한다.
- Agent에게 매번 같은 프롬프트를 주지 말고, **`@docs/DevOps/README.md`** 또는 하위 규칙 파일을 멘션한다.
