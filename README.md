# Pair Archive

자컾·페어 기록을 페어별로 모아 두는 개인 백업 사이트예요. 파일 하나(`index.html`)로 돌아가고, 서버가 필요 없어요.

A single-file personal archive for original-character pairs: photos, tweets, writing, and checklists, organized per pair. Records can be synced to a **private** GitHub repository.

## 기능

- **페어별 보기**: 페어마다 타임라인, 사진, 트윗, 글, 체크리스트, 프로필 탭
- **사진**: 카테고리 폴더로 분류, 컴퓨터 폴더째 올리기, 사진마다 설명, 낱장 모아보기
- **트윗**: 글만 트윗 모양으로 보관, 답글·인용·타래 지원, 여러 개 한꺼번에 붙여넣기
- **글**: AO3 HTML·EPUB, PDF, Word(.docx), TXT를 넣으면 같은 읽기 양식으로 정리. AO3 글은 팬덤·커플링·등급·요약·작가 노트·챕터·기울임까지 그대로, 연재 중인 글은 다시 넣으면 업데이트. 목차, 읽기 설정, 이어 읽기, TXT로 받기
- **체크리스트**: 구글 시트에서 복사해 붙여 넣으면 색·합친 칸·체크박스 그대로 표시, .xlsx/.csv 올리기, 시트 링크 첨부
- **꾸미기**: 페어마다 글꼴(내 글꼴 올리기 포함), 색, 머리 띠 무늬, 커버 이미지 크기·위치, 배경 무늬, 카드·탭 모양, 프리셋, CSS 직접 넣기
- **음악**: 페어마다 재생 목록(mp3·m4a·ogg·wav·flac 파일, 유튜브 링크), 작은 플레이어, 반복·섞어 듣기, 페어에 들어오면 자동 재생
- **AU**: 페어마다 AU(세계관)를 만들고 설정 메모를 적어 두고, 기록을 AU별로 모아 보기
- **시리즈**: 글을 시리즈로 묶어 순서대로 읽기, 읽기 화면에서 이전 편/다음 편
- **밑줄 긋기**: 읽다가 좋은 문장에 밑줄을 긋고 '밑줄 그은 문장'으로 모아 보기
- **다가오는 날**: 캐릭터 생일, 직접 넣은 기념일, D+100 단위와 매년 주년을 홈에서 알려 주기
- **휴지통**: 지운 기록과 페어를 30일 동안 보관하고 되살리기
- **순서 바꾸기**: 홈의 페어 순서를 바꾸고 맨 앞에 고정하기
- **잠금 비밀번호**: 사이트를 열 때 비밀번호 묻기, 복구 코드, 자리 비움 잠금
- **달력**: 페어마다 월 달력에 기록과 생일·기념일 표시, 날짜를 누르면 그날 기록
- **여러 개 선택**: 기록을 골라 AU·태그·가리기·폴더·즐겨찾기를 한꺼번에 바꾸거나 휴지통으로
- **트윗 한 장씩 보기**: 트윗을 한 장씩 크게 띄워 옆으로 넘겨 보기 (타래는 한 장에)
- **가리기**: 스포일러·민감한 내용은 목록에서 가려 두고 눌러야 보이기
- **태그 고르기**: 이미 쓴 태그를 드롭다운에서 골라 넣기
- **GitHub에 저장**: 기록과 사진을 비공개 저장소에 저장하고 다른 기기에서 불러오기, 자동 저장
- **그 밖에**: 통합 검색, 태그, 즐겨찾기, 디데이, 지난 오늘, 전체 백업 .zip

## 저장소 두 개로 쓰기 (추천)

| 저장소 | 공개 여부 | 들어 있는 것 |
| --- | --- | --- |
| `pair-archive` (이 저장소) | 공개 | 사이트 코드만. 기록은 없어요 |
| `pair-archive-data` | **비공개** | 내 기록과 사진 (`data/` 폴더) |

사이트 코드는 기록이 하나도 들어 있지 않아서 공개해도 괜찮아요. 무료 계정의 GitHub Pages는 공개 저장소만 열 수 있으니, 코드는 공개 저장소에 두고 기록만 비공개 저장소에 두면 휴대폰에서도 같은 주소로 쓸 수 있어요. 친구가 이 주소를 열어도 빈 사이트만 보여요.

### 1. 사이트 열기 (GitHub Pages)

1. 이 저장소의 **Settings › Pages**에서 Branch를 `main`, 폴더를 `/ (root)`로 정하고 저장해요.
2. 잠시 뒤 `https://<아이디>.github.io/pair-archive/` 주소로 열려요.

### 2. 기록용 비공개 저장소와 토큰 만들기

1. GitHub에서 **Private** 저장소를 새로 만들어요. 예: `pair-archive-data`
2. 프로필 › **Settings › Developer settings › Personal access tokens › Fine-grained tokens › Generate new token**
3. **Repository access**: *Only select repositories* → `pair-archive-data` 선택
4. **Permissions › Repository permissions › Contents**: *Read and write*
5. 만든 토큰을 복사해 둬요.

### 3. 사이트에 연결하기

사이트의 **설정 › GitHub에 저장**에서 저장소(`아이디/pair-archive-data`)와 토큰을 넣고 **연결 확인**을 눌러요.

- **지금 저장**: 이 브라우저의 기록을 저장소로 올려요. 맨 위 GitHub 버튼으로도 저장할 수 있어요.
- **불러오기**: 저장소의 기록을 이 브라우저로 가져와요. 새 기기에서 처음 연결했을 때 눌러 주세요.
- **자동 저장**: 기록을 바꾸면 15초 뒤에 저장돼요.
- 다른 기기에서 더 새로 저장한 기록이 있으면 위쪽에 알림이 떠요. 덮어쓰기 전에 꼭 확인해 주세요.
- 저장할 때마다 커밋이 하나씩 남아서, GitHub에서 예전 상태를 찾아볼 수 있어요.

## 알아 두기

- 토큰은 연결한 브라우저에만 저장되고, 어떤 저장소에도 올라가지 않아요. 공용 컴퓨터에서는 다 쓰고 **연결 끊기**를 눌러 주세요.
- 연결한 저장소가 공개 저장소면 연결을 막아요.
- GitHub에 연결하지 않으면 기록은 지금 쓰는 브라우저(IndexedDB)에만 남아요. 설정의 **전체 백업 받기 (.zip)** 로 따로 보관할 수도 있어요.

## 사용한 라이브러리 (CDN)

- [pdf.js](https://mozilla.github.io/pdf.js/): PDF 글자 추출
- [JSZip](https://stuk.github.io/jszip/): 백업 .zip 만들기
- [SheetJS](https://sheetjs.com/): .xlsx 시트 읽기
- [mammoth](https://github.com/mwilliamson/mammoth.js): Word(.docx) 글 읽기
- Google Fonts: Hahmlet, IBM Plex Sans KR, Gowun Dodum, Nanum Myeongjo, Gaegu, Jua
