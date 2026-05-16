# Yoojin Lee 웹사이트 수정 가이드

이 문서는 Yoojin Lee 개인 연구 웹사이트를 나중에 수정하거나 Codex에게 수정 요청할 때 참고하기 위한 한글 관리 문서입니다.

## 1. 프로젝트 개요

- 웹사이트 목적: Yoojin Lee의 개인 연구 웹사이트
- GitHub Pages 주소: <https://yjinbio.github.io/>
- GitHub 저장소: <https://github.com/yjinbio/yjinbio.github.io>
- 로컬 작업 디렉토리: `~/Desktop/yoojin`
- 웹사이트 본문 콘텐츠 언어: 주로 polished academic English
- 관리/수정 안내 문서 언어: 한국어

이 웹사이트는 Bioengineering, Immunology, Biomaterials, Immunoengineering 분야 연구자 프로필에 맞춘 정적 GitHub Pages 사이트입니다. 별도 빌드 과정 없이 `index.html`, CSS, 이미지, PDF 파일만으로 동작합니다.

## 2. 주요 파일 구조 설명

```text
~/Desktop/yoojin/
  index.html
  README.md
  WEBSITE_EDITING_GUIDE_KR.md
  assets/
    css/
      style.css
    files/
      Yoojin_Lee_CV.pdf
    images/
      profile/
        yoojin-lee.jpg
      research/
        phagocytosis.jpg
        trogocytosis.jpg
        mps.jpg
```

### `index.html`

웹사이트의 메인 콘텐츠 파일입니다. 브라우저에서 보이는 대부분의 텍스트와 섹션 구조가 이 파일에 들어 있습니다.

포함된 주요 섹션:

- Landing / Hero
- About
- Research Interests
- News
- Research Projects
- Education
- Research Experience
- Conferences
- Patent
- Skills
- Contact

웹사이트 문구, 링크, 섹션 순서, 항목 추가/삭제는 대부분 `index.html`에서 수정합니다.

### `assets/css/style.css`

전체 디자인과 레이아웃을 담당하는 CSS 파일입니다.

주요 역할:

- 글꼴, 색상, 간격, 배경색
- 데스크톱/모바일 반응형 레이아웃
- 상단 navigation 스타일
- hero/profile 영역 스타일
- 프로필 사진 크기와 둥근 모서리 스타일
- Research Project 카드 스타일
- Contact 링크 버튼 스타일

디자인, 배치, 모바일 표시, 이미지 크기 문제는 주로 이 파일에서 수정합니다.

### `assets/images/profile/yoojin-lee.jpg`

웹사이트 상단 hero/profile 영역에 표시되는 프로필 사진입니다.

사진을 교체할 때는 같은 파일명으로 덮어쓰면 `index.html`을 수정하지 않아도 됩니다.

### `assets/images/research/`

Research Projects 섹션에 표시되는 연구 프로젝트 이미지가 들어 있는 폴더입니다.

현재 주요 이미지 경로:

- `assets/images/research/phagocytosis.jpg`
- `assets/images/research/trogocytosis.jpg`
- `assets/images/research/mps.jpg`

필요할 때 실제 연구 도식, 현미경 이미지, 실험 플랫폼 이미지 등으로 교체할 수 있습니다.

### `assets/files/Yoojin_Lee_CV.pdf`

웹사이트의 CV 링크에 연결되는 공개용 CV 파일입니다.

중요: 이 파일은 웹사이트 방문자가 열람할 수 있는 공개 파일입니다. 공개용 CV에는 전화번호 등 민감한 개인정보를 제거하는 것을 권장합니다.

### `README.md`

프로젝트의 기본 설명, 로컬 실행 방법, GitHub Pages 배포 방법을 담은 영문 안내 문서입니다.

저장소를 처음 보는 사람이나 GitHub Pages 배포 절차를 확인할 때 참고합니다.

## 3. 자주 수정할 항목별 안내

### 자기소개 문구 수정

수정 파일: `index.html`

About 섹션의 문단을 수정하면 됩니다. 웹사이트 본문은 영어로 유지하고, 학술적이면서 간결한 톤을 권장합니다.

### Research Interests 수정

수정 파일: `index.html`

`Research Interests` 섹션의 bullet list를 수정합니다. 관심 분야는 너무 길게 쓰기보다 핵심 키워드 중심으로 유지하는 것이 좋습니다.

### News 항목 추가/수정

수정 파일: `index.html`

`News` 또는 `Recent Updates` 섹션의 timeline list에 항목을 추가하거나 수정합니다. 날짜 형식은 기존과 비슷하게 `Nov. 2025`, `Apr. 2025`처럼 유지합니다.

### Research Projects 수정

수정 파일: `index.html`

`Selected Projects` 섹션의 project card를 수정합니다. 각 프로젝트는 보통 다음 정보를 포함합니다.

- Title
- Status
- Description
- Keywords
- Image

프로젝트 설명은 polished academic English로 작성하고, 연구 성과를 과장하지 않도록 주의합니다.

### Education 수정

수정 파일: `index.html`

`Education` 섹션에서 학교명, 학위명, 기간, 위치를 수정합니다. CV와 불일치하지 않게 관리하는 것이 중요합니다.

### Research Experience 수정

수정 파일: `index.html`

`Research Experience` 섹션의 연구실, 직함, 기간, 지도교수, 주요 업무 bullet을 수정합니다. 경력 기간과 소속명은 CV와 일치시키는 것을 권장합니다.

### Conferences 추가

수정 파일: `index.html`

`Conferences` 섹션에 새 conference entry를 추가합니다. 발표 제목, 발표 형식, 장소, 날짜를 확인한 뒤 추가합니다.

### Patent 정보 수정

수정 파일: `index.html`

`Patent` 섹션에서 특허 제목, 역할, 출원 상태, 기관, 연도를 수정합니다. 출원번호나 등록번호를 공개해도 되는지 먼저 확인하는 것이 좋습니다.

### Skills 수정

수정 파일: `index.html`

`Skills` 섹션에서 Laboratory, Programming, Languages 항목을 수정합니다. 과도하게 긴 목록보다는 연구 포지션 지원에 유용한 핵심 기술을 유지하는 것이 좋습니다.

### 프로필 사진 교체

수정 파일:

- `assets/images/profile/yoojin-lee.jpg`
- 필요 시 `assets/css/style.css`

새 사진을 같은 경로와 파일명으로 교체하면 됩니다. 사진 비율이 크게 바뀌어 얼굴이 잘리거나 모바일에서 어색하게 보이면 `assets/css/style.css`의 `.profile-photo` 스타일을 조정합니다.

### CV PDF 교체

수정 파일: `assets/files/Yoojin_Lee_CV.pdf`

새 공개용 CV 파일을 같은 이름으로 덮어쓰면 됩니다. 파일명이나 경로를 바꾸는 경우에는 `index.html`의 CV 링크도 함께 수정해야 합니다.

### Google Scholar / ORCID 링크 추가

수정 파일: `index.html`

hero 영역의 profile links 근처에 있는 Google Scholar / ORCID placeholder를 실제 링크로 바꾸면 됩니다. Contact 영역에도 같은 스타일로 추가할 수 있습니다.

### 연구 이미지 교체

수정 파일:

- `assets/images/research/phagocytosis.jpg`
- `assets/images/research/trogocytosis.jpg`
- `assets/images/research/mps.jpg`
- 필요 시 `assets/css/style.css`

같은 파일명으로 이미지를 교체하면 `index.html` 수정 없이 반영됩니다. 이미지가 잘리거나 비율이 어색하면 `.project-card img` 스타일을 조정합니다.

## 4. 로컬 미리보기 방법

터미널에서 다음 명령어를 실행합니다.

```bash
cd ~/Desktop/yoojin
python3 -m http.server 8000
```

브라우저에서 다음 주소를 엽니다.

```text
http://localhost:8000
```

포트 `8000`이 이미 사용 중이면 다른 포트를 사용할 수 있습니다.

```bash
python3 -m http.server 8001
```

이 경우 브라우저에서 다음 주소를 엽니다.

```text
http://localhost:8001
```

## 5. GitHub Pages 업데이트 방법

수정 후 배포할 때는 다음 명령어를 사용합니다.

```bash
cd ~/Desktop/yoojin
git status
git add .
git commit -m "Update website"
git push
```

`git push`가 완료된 뒤 보통 몇 분 안에 GitHub Pages 사이트에 반영됩니다.

배포 주소:

```text
https://yjinbio.github.io/
```

반영이 늦어지는 경우 GitHub 저장소의 Actions 또는 Pages 설정에서 배포 상태를 확인합니다.

## 6. 개인정보 주의사항

- 전화번호는 웹사이트에 노출하지 않는 것을 권장합니다.
- CV PDF에 전화번호가 들어 있으면 웹사이트 방문자가 해당 정보를 볼 수 있습니다.
- 공개용 CV는 전화번호 제거 버전을 사용하는 것을 권장합니다.
- 원본 CV나 Research Summary PDF를 프로젝트 루트 디렉토리에 그대로 두면 `git add .` 실행 시 GitHub에 올라갈 수 있으므로 주의해야 합니다.
- 공개하고 싶지 않은 파일은 git에 추가하지 않거나 `.gitignore`에 넣어야 합니다.
- 이메일, LinkedIn, CV처럼 공개해도 되는 정보만 웹사이트에 표시하는 것이 좋습니다.
- 특허 출원번호, 논문 원고, 미공개 연구 이미지 등은 공개 가능 여부를 확인한 뒤 올려야 합니다.

## 7. Codex 수정 요청 예시 프롬프트

### 예시 1: News 추가

```text
WEBSITE_EDITING_GUIDE_KR.md를 참고해서 웹사이트를 수정해주세요. index.html의 News 섹션에 다음 항목을 추가해주세요: [날짜]: [내용]. 기존 스타일과 톤을 유지하고, 수정 후 한국어로 변경 파일을 요약해주세요.
```

### 예시 2: Research project 수정

```text
Research Projects 섹션에서 [프로젝트명] 설명을 다음 내용으로 자연스럽게 다듬어주세요: [내용]. 학술적이고 간결한 영어 문체를 유지해주세요.
```

### 예시 3: CV 교체

```text
assets/files/Yoojin_Lee_CV.pdf를 새 공개용 CV로 교체했습니다. CV 링크가 정상적으로 연결되는지 확인하고 README 또는 관련 설명이 필요하면 업데이트해주세요.
```

### 예시 4: 프로필 사진 교체

```text
assets/images/profile/yoojin-lee.jpg를 새 사진으로 교체했습니다. 이미지 비율과 모바일 표시가 자연스러운지 확인하고 필요한 CSS를 조정해주세요.
```

### 예시 5: Google Scholar / ORCID 추가

```text
Google Scholar 링크와 ORCID 링크를 추가해주세요. hero/contact 영역에 Email, LinkedIn, CV와 같은 스타일로 자연스럽게 배치해주세요.
```

### 예시 6: 전체 점검

```text
웹사이트 전체를 점검해주세요. 모바일 반응형, 링크 동작, 오타, 중복 정보, 개인정보 노출 여부를 확인하고 필요한 최소 수정만 반영해주세요.
```

## 8. 작업 원칙

- 제공되지 않은 논문, 수상, 소속, 링크는 임의로 만들지 않습니다.
- 웹사이트 본문은 polished academic English를 유지합니다.
- 작업 요약과 설명은 한국어로 작성합니다.
- 미니멀하고 학술적인 스타일을 유지합니다.
- 불필요한 외부 스크립트나 무거운 프레임워크를 추가하지 않습니다.
- 전화번호 등 민감한 개인정보는 새로 노출하지 않습니다.
- 기존 디자인과 파일 구조를 크게 바꾸기보다 필요한 부분만 정확히 수정합니다.
- 배포 전에는 로컬 미리보기로 링크, 이미지, 모바일 표시를 확인하는 것을 권장합니다.
