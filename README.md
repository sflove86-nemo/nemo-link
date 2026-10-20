# 내 링크 페이지 (정적 사이트)

DB·로그인 없이 `links.json` 하나로 동작하는 개인용 링크 페이지입니다.

## 파일
- `index.html` : 공개 페이지
- `links.json` : 프로필/링크/색상 데이터 (여기만 고치면 됨)
- `admin.html` : 링크 편집기 (수정 후 links.json 다운로드 → 덮어쓰기)

## 로컬 실행
```
python3 -m http.server 8000
```
브라우저에서 http://localhost:8000 (편집기는 /admin.html)

## 무료 배포 (택1)
- **Cloudflare Pages**: GitHub 저장소 연결 → 빌드 명령 없음, 출력 폴더 `/` → 개인/상업 모두 무료
- **GitHub Pages**: 저장소 Settings → Pages → main 브랜치 선택
- Vercel Hobby도 가능하나 수익 용도면 약관상 Pro 필요

## 참고
- admin.html은 비공개 보호가 없어요. 배포본에서 숨기려면 배포 시 admin.html을 빼고 로컬에서만 쓰세요.
