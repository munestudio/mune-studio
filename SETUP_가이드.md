# MUNE STUDIO 홈페이지 — 관리자 페이지 연결 가이드

이 폴더는 그냥 파일이 아니라, **직접 포트폴리오를 올리고 내리는 관리자 페이지(/admin)가 포함된 완전한 웹사이트**예요.
아래 순서대로 딱 한 번만 설정해두면, 그 다음부터는 저(Claude)한테 말할 필요 없이 대표님이 직접 사진을 올리고 몇 초~1분 안에 실제 홈페이지에 반영돼요.

무료로 진행되고, 코딩 지식은 필요 없어요. 총 15~20분 정도 걸려요.

---

## 1단계. GitHub에 이 폴더 올리기

1. github.com 에서 무료 계정 만들기 (이미 있으면 로그인)
2. 오른쪽 위 `+` → `New repository` 클릭
3. Repository name에 `mune-studio` 입력 → `Public` 선택 → `Create repository`
4. 생성된 저장소 페이지에서 `Add file` → `Upload files` 클릭
5. 이 폴더(mune-site) 안에 있는 **파일과 폴더를 전부** 끌어다 놓기 (index.html, admin 폴더, content 폴더, images 폴더 전부)
6. 아래로 내려서 `Commit changes` 클릭

## 2단계. Netlify로 사이트 배포하기

1. netlify.com 에서 무료 계정 만들기 (GitHub 계정으로 가입하면 더 빠름)
2. `Add new site` → `Import an existing project` → `GitHub` 선택 → 방금 만든 `mune-studio` 저장소 선택
3. 설정은 그대로 두고 `Deploy site` 클릭 → 1분 정도 기다리면 `xxxx.netlify.app` 주소로 사이트가 열림
4. (선택) Site settings → Domain management 에서 갖고 있는 도메인(munestudio.kr 등) 연결 가능

## 3단계. 관리자 로그인 기능 켜기 (Identity + Git Gateway)

1. Netlify 사이트 대시보드 → 상단 메뉴 `Identity` 클릭 → `Enable Identity` 클릭
2. `Identity` 탭 안의 `Registration` → `Edit settings` → `Invite only`로 변경 (아무나 가입 못 하게 막는 설정, 꼭 해주세요)
3. 같은 탭 아래쪽 `Services` → `Git Gateway` → `Enable Git Gateway` 클릭

## 4단계. 나 자신을 관리자로 초대하기

1. `Identity` 탭 → `Invite users` 버튼 클릭
2. 대표님 이메일(munestudio.creative@gmail.com) 입력 후 초대 보내기
3. 메일함 확인 → Netlify에서 온 초대 메일 열어서 `Accept the invite` 클릭
4. 비밀번호 설정하면 자동으로 관리자 페이지로 로그인됨

## 5단계. 실제로 포트폴리오 올리기

1. 브라우저 주소창에 `내사이트주소.netlify.app/admin` 입력 (직접 만든 도메인을 연결했다면 `munestudio.kr/admin`)
2. 로그인 후 왼쪽 메뉴에서 `포트폴리오` 클릭
3. `items` 목록에서 `+ Add` 버튼으로 새 작업물 추가 — 제목, 카테고리(브랜딩/상세페이지/컨텐츠디자인/로고디자인/패키지), 대표 이미지, 클라이언트/브랜드명, 연도, 상세 설명, 추가 이미지(갤러리)까지 입력
4. 오른쪽 위 `Publish` 버튼 클릭
5. 30초~1분 정도 지나면 실제 홈페이지의 포트폴리오 섹션에 자동으로 반영돼요 (새로고침만 하면 됨)

포트폴리오 카드를 클릭하면 비헨스 프로젝트처럼 대표 이미지·클라이언트·연도·설명·추가 이미지가 담긴 상세 창이 열려요. 클라이언트/연도/설명/추가 이미지는 비워둬도 되고, 나중에 언제든 채워 넣을 수 있어요.

순서를 바꾸거나 삭제하고 싶을 때도 같은 화면에서 항목을 끌어서 옮기거나 휴지통 아이콘으로 지우면 돼요.

---

막히는 부분 있으면 화면 캡처해서 저한테 보여주세요. 같이 확인해드릴게요.
