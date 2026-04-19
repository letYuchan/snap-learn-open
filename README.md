<div align="center">

# Snap Learn

**Claude Code 로 만든 걸 잊기 전에, 개념부터 다시 잡는다.**

macOS 앱 · 백그라운드에서 세션을 감시해 놓친 개념을 30초 학습 카드로 복원합니다.

[Download DMG](https://github.com/letYuchan/snap-learn-open/releases/latest) · [Features](#features) · [Install](#install) · [Privacy](#privacy)

![macOS](https://img.shields.io/badge/macOS-Apple%20Silicon-black?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)
![Stage](https://img.shields.io/badge/Stage-Alpha-orange?style=flat-square)

</div>

---

## Why

AI 도우미 덕에 **결과는 빨라졌는데**, 정작 **왜 그렇게 동작하는지** 설명이 안 되는 순간이 많아요. 다음 작업이 바로 이어지니 정리할 시간도 없고요. Snap Learn 은 그 격차를 백그라운드에서 메웁니다. **개발 흐름은 그대로.**

---

## Features

| | |
|---|---|
| 🔎 **자동 감시** | 세션 델타 tail → 의미 있는 순간에 30초 팝업 |
| 🎙 **면접 연습** | 1문1답 10회 티키타카 · 4축(정확성·깊이·트레이드오프·명료성) 채점 |
| 📚 **코어·트렌드** | Kleppmann 급 기초 + 최근 1~2년 실전 주제 자동 큐레이션 |
| 🗞 **뉴스 디지스트** | 관심사 기반 데일리, 1차 출처 우선 |
| 🧠 **AI 분석 리포트** | 능동 수행(면접·퀴즈)만으로 타입·강약점·미션 추출 |
| 🧾 **Notion 연동** | 로컬이 기본, Notion 은 옵션 |

---

## Install

1. **[DMG 다운로드](https://github.com/letYuchan/snap-learn-open/releases/latest)** → `Snap Learn.app` 을 `/Applications` 로 드래그
2. **Claude CLI 로그인** (별도 API 키 불필요)
   ```bash
   brew install anthropic/tap/claude
   claude login
   ```
3. 앱 실행 → 온보딩이 권한·저장 폴더 안내

> Apple Silicon 전용. Developer ID 서명됨.

---

## Privacy

- **로컬 우선** — 노트·면접·세션 모두 사용자 PC 에만 저장
- **본문 미기록** — Usage 로그는 글자 수만 저장, prompt/response 본문은 디스크에 남지 않음
- **Keychain** — Notion 토큰 등 민감 값은 macOS Keychain 에 저장
- **텔레메트리 없음** — 분석 SDK·크래시 리포터 미탑재

---

## Stack

Tauri 2 · React 18 · TypeScript 5 · Tailwind 4 · TanStack Query · Zustand · Claude CLI

---

## License

[MIT](./LICENSE) — Keep learning without breaking the flow.
