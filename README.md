# 외대HS어학원 도봉브랜치 홈페이지

정적 웹사이트(HTML/CSS/JS)라서 GitHub Pages로 무료로 호스팅할 수 있습니다.

## 파일 구성

| 파일 | 내용 |
|---|---|
| `index.html` | 홈페이지 본문 (문구 수정은 여기서) |
| `css/style.css` | 디자인 (색상, 글자 크기, 여백) |
| `js/main.js` | 모바일 메뉴, 스크롤 효과 |
| `assets/` | 사진, 로고, 파비콘 |
| `robots.txt` | 검색엔진 수집 허용 설정 |

## 아직 채워야 할 내용

`index.html`에서 `TODO`로 검색하면 위치를 찾을 수 있습니다.

- 주소, 운영시간
- 블로그 6개 글의 제목과 한 줄 소개

## GitHub Pages로 공개하기

1. GitHub에서 새 저장소를 **Public**으로 만듭니다.
2. 이 폴더 안의 파일을 모두 업로드합니다. (저장소 화면의 **Add file → Upload files**에 끌어다 놓기)
3. 저장소의 **Settings → Pages**에서 Source를 **Deploy from a branch**, Branch를 **main / (root)** 로 선택하고 저장합니다.
4. 1~2분 뒤 Pages 화면 위쪽에 사이트 주소가 표시됩니다.

## 학원 도메인 연결하기 (선택)

1. 가비아, Cloudflare 등에서 도메인을 구매합니다. (예: `hsdobong.kr`)
2. 도메인 관리 화면의 DNS 설정에 아래 레코드를 추가합니다.
   - `A` 레코드 4개: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` 레코드: 호스트 `www`, 값 `GitHub아이디.github.io`
3. GitHub 저장소의 **Settings → Pages → Custom domain**에 도메인을 입력하고 저장합니다.
4. 인증서가 발급되면 **Enforce HTTPS**를 체크합니다.

도메인을 연결한 뒤 `index.html`의 `og:image` 주소를 전체 주소(`https://도메인/assets/speech-contest-2026.jpg`)로 바꾸고 `sitemap.xml`을 추가하면 카카오톡 공유 미리보기와 검색 노출에 유리합니다.

## 검색 등록

- 네이버 서치어드바이저(searchadvisor.naver.com): 사이트 등록 후 소유 확인
- 구글 서치콘솔(search.google.com/search-console): 사이트 등록 후 소유 확인
