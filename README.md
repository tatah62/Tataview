# Tataview 🐶

[English below ↓](#tataview--english)

모두 안녕! 👋
**Tataview**는 논문이랑 노트를 **읽으면서 표시하는** 맥 앱이야.
md·PDF·워드·엑셀을 열어서 형광펜·밑줄·포스트잇을 붙이고, 인터뷰 전사 같은 표는 엑셀처럼 걸러보고, 옆에 붙어 있는 Claude한테 정리를 맡길 수 있어.

## ✅ 필요한 것
- **M칩 맥** (Apple Silicon), **macOS 13** 이상
- **[Claude Code](https://docs.anthropic.com/claude-code)** 설치 + 로그인 (앱 오른쪽 Claude 칸에서 써)
  - 터미널에서 `claude` 쳐서 실행되면 준비 끝!

## ⬇️ 받기
### [Tataview 0.5 다운로드 (dmg)](https://github.com/tatah62/Tataview/releases/download/v0.5/Tataview-0.5.dmg)
받은 `Tataview-0.5.dmg`를 열고 **Tataview를 Applications로 끌어다 놓으면** 끝이야.
처음 켤 때 **한국어 / English**를 고를 수 있어 (나중에 **보기 → 언어**에서 바꿔).
처음 열 때 경고가 뜨면 [설치 안내](설치_안내.md)를 봐줘. (다른 버전·바뀐 내용은 [Releases](https://github.com/tatah62/Tataview/releases))

## 📖 이런 앱이야

### 📄 읽기
- **md, PDF, 워드(docx), 엑셀(xlsx), CSV**를 열 수 있어
- 워드·엑셀·CSV는 읽기 좋게 바꿔서 보여줘 (원본은 그대로)
- 수식(LaTeX), 그림, 표도 예쁘게 보여
- **원본은 절대 안 바뀌어.** 표시하고 저장하면 Tataview 폴더에 사본이 따로 생겨

### 🖍 표시하기
- 글자를 드래그하면 작은 막대가 떠
  - **형광펜** 5색, **밑줄**
  - **포스트잇** 📝: 그 자리에 스티커를 붙이고, 누르면 큰 메모지가 떠
    - 굵게·기울임·제목·글자 크기, 목록·번호·체크박스·들여쓰기
    - 색 6가지, 연한 격자 무늬
- 아무 데나 **우클릭 → 여기에 포스트잇 붙이기** (빈 곳도 OK)
- 메모에 `#태그`를 달면 태그끼리 모아보고, **태그 그래프**로 어떤 문장이 어떤 태그로 묶였는지 한눈에 봐
- 칠한 곳에 마우스를 올리면 메모가 말풍선으로 떠
- 오른쪽 **하이라이트 칸**에 형광펜·밑줄·포스트잇이 다 모여 (필터로 골라보기, 내보내기)

### 📊 표 (인터뷰 전사, 정리용 표)
- 칸 제목 옆 **▾** = **엑셀식 필터**: 값을 골라서 그 줄만 보기, 정렬, 여러 칸 동시에
- 칸에 `a, b`처럼 코드를 여러 개 적으면 하나씩 따로 걸러져 (오픈 코딩할 때 좋아)
- **노트 칸**은 눌러서 바로 쓰고, 다른 칸은 **편집** 모드에서 고치기·줄/칸 추가
- **CSV로 내보내기** (엑셀에서 바로 열려)

### 🤖 옆에 붙어 있는 Claude
- 앱 오른쪽에 **Claude Code**가 바로 떠 있어 (한글 입력 OK)
- 파일은 직접 열어도 되고, Claude한테 말로 시켜도 돼. 시킨 결과는 앱에 바로 반영돼
- 💬 **이렇게 말하면 돼**
  - 📑 "다운로드에 있는 ○○ 논문 PDF 읽고, 섹션별로 세세하게 불릿포인트 요약본 만들어서 이 프로젝트에 넣어줘"
  - 🔍 "이 논문에서 연구 질문, gap, 방법, 주요 결과만 뽑아서 표로 정리해줘"
  - 📊 "이 엑셀 인터뷰 전사를 표로 바꿔서 theme 칸 하나 추가해줘"
  - 🏷 "이 프로젝트에서 #fear_to_speak 붙은 포스트잇이랑 문장 다 모아서 정리해줘"
  - 📝 "이 노트 너무 빽빽해. 문단 사이 간격 넓히고 소제목 달아서 읽기 좋게 정리해줘"
  - 🧮 (수식 스크린샷 붙이고) "이 식 풀이 과정 단계별로 md로 정리해줘"
  - 🗂 "새 프로젝트 '문헌 정리' 만들고, 미분류에 있는 논문 노트들 거기로 옮겨줘"
  - ✏️ "이 파일 이름 '2026_Kim_정독'으로 바꿔줘"
  - 💾 "저장해" (열린 파일 전부 저장)
  - 💌 "불편했던 거 정리해서 Tataview 피드백 보내줘"
- **스크린샷**을 ⌘V로 붙이면 미리보기가 뜨고, 질문 쓰고 Enter 치면 md로 기록하면서 물어봐
- 나눈 대화는 프로젝트별로 **자동으로 기억**해

### 💾 저장·파일
- **워드처럼** ⌘S로 저장. 저장 안 하고 닫으면 물어봐
- 프로젝트 폴더(폴더 안 폴더 OK), 끌어서 옮기기, 이름 바꾸기, 휴지통으로 보내기
- **A4 인쇄**(세로/가로), PDF로 저장

### 🎨 화면
- **언어**: 한국어 / English
- **테마**: 라이트·다크·겨울 밤 + 딸기 말차·겨울 아침·콘플라워·프로스트 앤 엠버·크리스마스, **직접 정하기**
  - 형광펜·포스트잇 색도 테마를 따라 바뀌어
- 패널마다 접기·펴기, 경계선 끌어서 너비 조절
- 기본 단축키 다 돼 (⌘N·⌘O·⌘S·⌘Z·⌘F·⌘B…, Ctrl도 OK)
- 처음 켜면 **사용법**이 떠 (나중엔 메뉴 Tataview → 사용법, ⌘/)

## 💌 피드백
불편한 점이나 아이디어가 있으면 편하게 보내줘!
- 앱 메뉴 **Tataview → 피드백 보내기…**
  - 고칠 점·버그·아이디어 중에 고르고 내용 쓰기
  - 📸 **스크린샷 첨부는 여기서!** "지금 화면 스크린샷 같이 보내기"를 체크하면 지금 화면이 같이 가
- 또는 오른쪽 Claude한테 이렇게 말해줘 (글로만 보내져)
  - 💬 "불편했던 거 정리해서 Tataview 피드백 보내줘"
  - 🐛 "표 필터가 가끔 안 풀려. 버그로 Tataview 피드백 보내줘"
  - 💡 "포스트잇 모아보는 화면 있으면 좋겠어. 아이디어로 Tataview 피드백 보내줘"

---

# Tataview 🐶 (English)

Hi everyone! 👋
**Tataview** is a Mac app for **reading papers and notes while marking them up**.
Open md, PDF, Word and Excel files, add highlights, underlines and sticky notes, filter tables like interview transcripts the way you would in Excel, and hand the tidying up to Claude right next to your document.

## ✅ What you need
- **An Apple Silicon (M-chip) Mac**, **macOS 13** or later
- **[Claude Code](https://docs.anthropic.com/claude-code)** installed and signed in (used in the Claude panel on the right)
  - If typing `claude` in Terminal starts it, you're all set!

## ⬇️ Download
### [Download Tataview 0.5 (dmg)](https://github.com/tatah62/Tataview/releases/download/v0.5/Tataview-0.5.dmg)
Open `Tataview-0.5.dmg` and **drag Tataview into Applications**. That's it.
On first launch you pick **English or 한국어** (you can change it later in **View → Language**).
If macOS warns you the first time, see the [install guide](설치_안내.md#tataview-install-guide-english). (Other versions and changes: [Releases](https://github.com/tatah62/Tataview/releases))

## 📖 What it does

### 📄 Reading
- Opens **md, PDF, Word (docx), Excel (xlsx) and CSV**
- Word, Excel and CSV are converted for easy reading (the original stays untouched)
- Math (LaTeX), images and tables look nice
- **Your originals never change.** When you mark something up and save, a separate copy is made in your Tataview folder

### 🖍 Marking up
- Drag over text and a small bar pops up
  - **Highlighter** in 5 colors, **underline**
  - **Sticky note** 📝: stick a note right there; click it to open a big note pad
    - Bold · italic · headings · text size, bullets · numbering · checkboxes · indent
    - 6 colors, light grid
- **Right-click anywhere → Stick a sticky note here** (empty space works too)
- Add `#tags` to notes to group them, and see which sentences share a tag in the **tag graph**
- Hover over a highlight to see its note in a bubble
- The **highlights panel** on the right collects all highlights, underlines and sticky notes (filter them, export them)

### 📊 Tables (interview transcripts, working tables)
- **▾** next to a column title = **Excel-style filter**: pick values to show only those rows, sort, filter several columns at once
- Write several codes in a cell like `a, b` and each one is filtered separately (great for open coding)
- Click a **note cell** to type right away; use **Edit** mode for other cells and to add rows/columns
- **Export as CSV** (opens straight in Excel)

### 🤖 Claude, right next to you
- **Claude Code** sits on the right side of the app
- Open files yourself or just ask Claude. Whatever it does shows up in the app right away
- 💬 **Things you can say**
  - 📑 "Read the ○○ paper PDF in Downloads and make a detailed section-by-section bullet summary in this project"
  - 🔍 "Pull out the research questions, gap, method and main findings of this paper into a table"
  - 📊 "Turn this Excel interview transcript into a table and add a theme column"
  - 🏷 "Gather every sticky note and sentence tagged #fear_to_speak in this project"
  - 📝 "This note is too dense. Add space between paragraphs and some subheadings"
  - 🧮 (paste a screenshot of a formula) "Write out the solution step by step in md"
  - 🗂 "Make a new project 'Literature' and move the paper notes from Unsorted there"
  - ✏️ "Rename this file to '2026_Kim_reading'"
  - 💾 "Save" (saves every open file)
  - 💌 "Sum up what bugged me and send Tataview feedback"
- Paste a **screenshot** with ⌘V to preview it, then type a question and press Enter to log it in md and ask Claude
- Conversations are **remembered automatically** per project

### 💾 Saving & files
- Save with ⌘S **like Word**. If you close without saving, Tataview asks
- Project folders (folders in folders OK), drag to move, rename, move to Trash
- **A4 printing** (portrait/landscape), save as PDF

### 🎨 Screen
- **Themes**: Light · Dark · Winter Night + Strawberry Matcha · Winter Morning · Cornflower · Frost & Ember · Christmas, and **Custom**
  - Highlighter and sticky-note colors follow the theme
- **Language**: English / 한국어
- Collapse each panel, drag borders to resize
- All the usual shortcuts (⌘N · ⌘O · ⌘S · ⌘Z · ⌘F · ⌘B…, Ctrl works too)
- A **guide** shows up on first launch (later: menu Tataview → How to use, ⌘/)

## 💌 Feedback
Bugs, ideas, anything annoying — send it anytime!
- App menu **Tataview → Send feedback…**
  - Pick something to fix · bug · idea, and write it down
  - 📸 **Attach screenshots here!** Check "Attach a screenshot of the current screen" to include what you see
- Or ask Claude on the right (text only)
  - 💬 "Sum up what bugged me and send Tataview feedback"
  - 🐛 "The table filter sometimes won't clear. Send it as a bug to Tataview feedback"
  - 💡 "It'd be nice to have a screen that collects all sticky notes. Send it as an idea to Tataview feedback"
