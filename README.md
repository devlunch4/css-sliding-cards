# CSS Sliding Cards 프로젝트

HTML과 CSS를 사용하여 제작한 반응형 카드 UI 프로젝트입니다.
카드를 선택하면 확장되면서 상세 정보가 부드럽게 표시됩니다.

## 목차

1. [주요 기능](#주요-기능)
2. [프로젝트 구조](#프로젝트-구조)
3. [HTML 구조](#html-구조)
4. [CSS 기술](#css-기술)
5. [실행 방법](#실행-방법)
6. [개발 환경](#개발-환경)
7. [배포](#배포)
8. [English-ver](#english-ver)


## 주요 기능

* **인터랙티브 카드 선택:** 클릭 시 카드가 확장되어 추가 정보 표시
* **부드러운 애니메이션:** 카드 확장 및 내용 표시 시 전환 효과 적용
* **반응형 레이아웃:** Flexbox 기반으로 다양한 화면 크기에 대응
* **JavaScript 불필요:** HTML과 CSS만으로 구현

## 프로젝트 구조

```
/css-sliding-cards
│
├─ index.html        # 웹페이지 구조 및 카드 요소
├─ style.css         # Flex 레이아웃, 카드 스타일, 애니메이션
├─ img1.png          # 카드 1 이미지
├─ img2.png          # 카드 2 이미지
├─ img3.png          # 카드 3 이미지
└─ img4.png          # 카드 4 이미지
```

## HTML 구조

* `.wrapper`: 전체 화면을 채우고 카드 레이아웃을 중앙에 배치
* `.container`: 여러 `.card` 요소를 가로로 정렬
* `.card`: 클릭 가능한 카드, 아이콘과 설명 포함. 숨겨진 radio `input`과 연결
* `.row`: 카드 내 아이콘과 설명을 가로 배치
* `.description`: 제목과 설명, 기본적으로 숨김 상태이며 선택 시 CSS 트랜지션으로 표시

## CSS 기술

* **Flexbox:** 카드 가로 레이아웃 및 내용 정렬
* **CSS 전환(transition):** 카드 확장과 설명 fade-in/슬라이드 업 효과
* **Radio input 활용:** `input:checked + label` 선택자를 이용한 카드 확장
* **Box-shadow & border-radius:** 카드에 깊이감과 둥근 모서리 적용
* **Background-image:** 카드 시각적 콘텐츠

## 실행 방법

1. `index.html`을 최신 웹 브라우저에서 열기
2. Project IDX 환경에서는 웹 서버가 자동 실행됨. 우측 상단 미리보기 아이콘 클릭 후 'web' 선택
3. GitHub Pages 등에서 정적 호스팅 가능

## 개발 환경

* **Nix 기반 환경**에서 패키지 및 개발 도구 관리
* `.idx/dev.nix` 파일에서 필요한 패키지 및 VS Code 확장 관리 가능
* 순수 프론트엔드 구현으로 별도 빌드 도구 필요 없음

## 배포

프로젝트는 GitHub Pages를 통해 배포되었습니다.  
[https://devlunch4.github.io/css-sliding-cards/](https://devlunch4.github.io/css-sliding-cards/)


---

## English-Ver

---


# CSS Sliding Cards Project

A responsive card UI project implemented with HTML and CSS.
Cards expand on selection, revealing detailed content with smooth transitions.

## Table of Contents

1. [Features](#features)
2. [Project Structure](#project-structure)
3. [HTML Structure](#html-structure)
4. [CSS Techniques](#css-techniques)
5. [How to Run](#how-to-run)
6. [Development Environment](#development-environment)
7. [Deployment](#deployment)

## Features

* **Interactive card selection:** Cards expand on click to show additional information
* **Smooth animations:** Transition effects for expanding cards and revealing content
* **Responsive layout:** Flexbox ensures proper alignment on different screen sizes
* **No JavaScript required:** Fully functional UI using HTML and CSS only

## Project Structure

```
/css-sliding-cards
│
├─ index.html        # Webpage structure and card elements
├─ style.css         # Flex layout, card styling, and animations
├─ img1.png          # Image for Card 1
├─ img2.png          # Image for Card 2
├─ img3.png          # Image for Card 3
└─ img4.png          # Image for Card 4
```

## HTML Structure

* `.wrapper`: Full-screen container centering the card layout
* `.container`: Holds multiple `.card` elements in a horizontal flex layout
* `.card`: Clickable card with icon and description, linked to a hidden radio `input`
* `.row`: Organizes icon and description side by side
* `.description`: Heading and paragraph content, hidden by default and revealed via CSS transitions

## CSS Techniques

* **Flexbox:** Horizontal layout for cards and alignment of content
* **CSS transitions:** Smooth expansion and fade-in/slide-up of card content
* **Radio input trick:** Card expansion using `input:checked + label` selector
* **Box-shadow & border-radius:** Adds depth and rounded corners to cards
* **Background images:** Visual content for each card

## How to Run

1. Open `index.html` in any modern web browser
2. In Project IDX, the web server starts automatically. Click the preview icon and select 'web'
3. Can also be hosted statically via GitHub Pages

## Development Environment

* **Nix-managed environment** for dependencies and tools
* Packages and VS Code extensions configurable via `.idx/dev.nix`
* Pure front-end implementation, no build tools required

## Deployment

The project is deployed via GitHub Pages.  
[https://devlunch4.github.io/css-sliding-cards/](https://devlunch4.github.io/css-sliding-cards/)

