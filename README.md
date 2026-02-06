# 솔라나-이더리움 가격 추적기

이 저장소는 단일 정적 페이지(`index.html`)로 동작합니다.

## GitHub에 올리기

```bash
git remote add origin https://github.com/<YOUR_ID>/<REPO>.git
git push -u origin <BRANCH_NAME>
```

> 저장소를 **Private**로 생성하면 코드 접근은 본인만 가능합니다.

## "나만 접속" 가능한 배포 방법(권장)

GitHub Pages 단독으로는 강한 인증 보호를 걸기 어렵기 때문에,
**Cloudflare Zero Trust Access**로 보호하는 구성을 권장합니다.

1. Cloudflare Pages에 이 GitHub 저장소 연결
2. Pages 도메인 생성
3. Zero Trust Access에서 애플리케이션 생성
4. 정책을 내 이메일 1개만 허용

이렇게 하면 사이트 URL을 알아도 인증된 계정(본인)만 접속할 수 있습니다.

## 로컬 실행

```bash
python3 -m http.server 4173
```

브라우저에서 `http://localhost:4173` 접속.
