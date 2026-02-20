# Gemini CLI for Everyone (GC4E): AI 활용의 기술

*Carl Vellotti의 "Claude Code for Everyone"을 원작으로 하며, Sujeong Lim이 Gemini CLI용으로 각색 및 최적화했습니다.*

## 이 코스는 무엇인가요?

코딩 경험이 전혀 없어도 실제 시나리오를 통해 Gemini CLI를 배우는 실습형 인터랙티브 코스입니다.

직접 해보면서 배웁니다 - Gemini CLI가 터미널에서 직접 가르쳐줍니다. 각 레슨은 가이드형 인터랙티브 경험입니다.

## 시나리오

여러분은 **Basecamp Coffee**의 새로운 매니저입니다. 이 지역 체인점은 충성도 프로그램이 어려움을 겪고 있습니다. 모듈 1과 2를 통해 Gemini CLI를 사용해 문제를 분석하고, 인사이트를 발견하며, 실제 솔루션을 구축할 것입니다.

## 코스 구조

### 모듈 1: 기초 (파일과 함께 작업하기)
| 레슨 | 배울 내용 |
|------|-----------|
| 1.1 소개 | 환영 및 Basecamp Coffee 시나리오 설정 |
| 1.2 파일 탐색 | 파일 탐색, Cursor 워크스페이스 설정 |
| 1.3 파일 작업 | @ 멘션: 파일, 폴더, 템플릿, 이미지, 웹 |
| 1.4 명령어 및 탐색 | 슬래시 명령어, 커스텀 명령어(TOML), 승인 모드, Chain-of-Thought |
| 1.5 에이전트 | 병렬 처리를 위한 서브에이전트 |
| 1.6 커스텀 서브에이전트 | .gemini/agents/로 팀원 만들기 |
| 1.7 GEMINI.md | 프로젝트 지속 메모리 및 /memory 명령어 |
| 1.8 고급 기능 | 복습, 툴킷 표, 고급 기능 미리보기 |

### 모듈 2: 바이브 코딩 (처음부터 빌드하기)
| 레슨 | 배울 내용 |
|------|-----------|
| 2.1 설정 | 계획 → 빌드 → 반복 → 저장 → 배포 루프 |
| 2.2 계획 | 커피 성격 퀴즈 요구사항 정의 |
| 2.3 빌드 및 반복 | Next.js로 빌드하고 스크린샷으로 반복 |
| 2.4 GitHub | GitHub CLI로 GitHub에 저장 |
| 2.5 런칭 | Vercel에 배포 - 실제 URL, 실제 앱 |

## 시작하기

### 사전 요구사항
- [Gemini CLI](https://geminicli.com/docs) 설치 및 설정
- 터미널 (macOS 터미널, Windows PowerShell, 또는 Linux 터미널)
- 호기심 (코딩 경험 불필요!)

### 코스 시작

1. 터미널 열기
2. 이 폴더로 이동: `cd path/to/complete-course`
3. Gemini CLI 실행: `gemini`
4. 첫 번째 레슨 시작: `/start-1-1`

이게 전부입니다! Gemini CLI가 거기서부터 안내해 드립니다.

## 폴더 구조

```
complete-course/
├── .gemini/                    # Gemini CLI 설정
│   ├── SCRIPT_INSTRUCTIONS.md  # 교육 행동 가이드라인
│   ├── commands/               # 커스텀 슬래시 명령어 (TOML)
│   │   ├── start-1-1.toml     # ... start-2-5.toml까지
│   │   └── ...
│   └── agents/                 # 커스텀 서브에이전트 정의
│       ├── barista-lead.md    # 현장 운영 관점
│       ├── exec.md            # 임원/ROI 관점
│       └── product-designer.md # UX/디자인 관점
├── lesson-modules/             # 레슨 스크립트 (GEMINI.md 파일)
│   ├── 1.1-introduction/
│   ├── 1.2-file-exploration/
│   ├── ...
│   └── 2.5-go-live/
├── company-context/            # Basecamp Coffee 배경 정보
├── inherited-chaos/            # 분석할 혼잡한 파일들
├── templates/                  # 문서 템플릿
├── attachments/                # 이미지 및 미디어
├── course-structure.json       # 코스 메타데이터
└── README.md                   # 이 파일
```

## 다루는 주요 Gemini CLI 기능

- **GEMINI.md** - 계층적 컨텍스트를 통한 지속적인 프로젝트 메모리
- **커스텀 명령어** - `.gemini/commands/`의 TOML 기반 단축키
- **커스텀 서브에이전트** - `.gemini/agents/`의 전문화된 AI 페르소나
- **승인 모드** - Shift+Tab으로 순환: 기본 → 자동 편집 → 계획
- **Chain-of-Thought** - 프롬프팅 및 GEMINI.md 지시사항을 통한 심층 추론
- **/memory** - 지속적인 컨텍스트 보기, 추가, 새로고침
- **/rewind** - 변경사항 취소 (Esc×2)
- **/resume** - 이전 세션 계속하기
- **정책 엔진** - 세밀한 도구 실행 제어

## 문서

포괄적인 Gemini CLI 문서는 **[geminicli.com/docs](https://geminicli.com/docs)**를 방문하세요.

## 크레딧

- **원본 코스:** [Carl Vellotti](https://x.com/carlvellotti)의 "Claude Code for Everyone"
- **Gemini CLI 각색:** Sujeong Lim
