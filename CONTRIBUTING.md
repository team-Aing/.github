# 기여 가이드

## 프로젝트 올리기

1. 올가에 새 레포를 만들거나, 개인 레포를 Fork 또는 Transfer 합니다.
2. README에 최소한 아래 내용을 적어 주세요.
   - 프로젝트 한 줄 소개
   - 실행 방법
   - 사용 기술
   - 피드백 받고 싶은 부분
3. `.env`, API 키, 토큰 같은 비밀 정보와 모델 가중치 같은 대용량 파일은 커밋하지 마세요. `.gitignore`를 먼저 확인하세요.

## 피드백 주기

- **의견, 개선 아이디어**: 해당 레포 Issues에서 `피드백` 템플릿 사용
- **버그 발견**: `버그 제보` 템플릿 사용
- **코드 수정 제안**: Fork → 브랜치 생성 → Pull Request
  - 올가 기본 권한이 Read라서 다른 사람 레포에는 직접 push할 수 없습니다.

## Pull Request 흐름

```bash
# 1. 원본 레포를 Fork한 뒤 내 Fork를 클론
git clone https://github.com/<내-아이디>/<레포>.git
cd <레포>

# 2. 작업 브랜치 생성
git switch -c fix/짧은-설명

# 3. 커밋 후 내 Fork로 푸시
git add .
git commit -m "fix: 짧은 설명"
git push origin fix/짧은-설명
```

4. GitHub에서 원본 레포로 Pull Request를 엽니다.
5. 머지 여부는 레포 주인이 결정합니다.

## 커밋 메시지 규칙 (권장)

| 타입 | 용도 |
| --- | --- |
| `feat` | 새 기능 |
| `fix` | 버그 수정 |
| `docs` | 문서 수정 |
| `refactor` | 동작 변화 없는 코드 개선 |
| `test` | 테스트 추가, 수정 |
| `chore` | 설정, 의존성 등 기타 |

예: `feat: 로그인 API 추가`
