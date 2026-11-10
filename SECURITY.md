# 보안 정책

## 비밀 정보 유출을 발견했다면

API 키, 토큰, 비밀번호 등이 레포에 올라간 것을 발견하면 **공개 Issue에 적지 말고**
레포 주인이나 올가 오너에게 개인 메시지로 알려 주세요.

## 내 키가 유출됐다면 (레포 주인)

1. 해당 키를 **즉시 폐기(revoke)하고 새로 발급**하세요. 커밋을 지워도 기록에 남아 있을 수 있습니다.
2. `.gitignore`에 `.env` 등을 추가하고, 코드에서는 환경변수로 불러오세요.

## 예방

- `.env`는 커밋하지 않고 `.env.example`만 올리기
- 레포 Settings → Advanced Security에서 Secret scanning, Push protection 켜기 (public 레포는 무료)
