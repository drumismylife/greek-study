# 헬라어 I 학습 앱 — GitHub Pages 배포 가이드

## 📁 폴더 구조

```
my-greek-app/          ← GitHub 저장소 루트
├── index.html         ← 헬라어_학습앱.html 을 이 이름으로 저장
├── audio/             ← MP3 파일 220개 전부 여기에
│   ├── alph_alpha.mp3
│   ├── alph_beta.mp3
│   ├── vv1_luo.mp3
│   ├── vn_logos.mp3
│   └── ... (220개)
└── README.md
```

## 🚀 배포 방법 (5단계)

### 1. GitHub 저장소 생성
- github.com → New repository
- 이름: `greek-study` (또는 원하는 이름)
- Public 선택 → Create repository

### 2. 파일 업로드
- `헬라어_학습앱.html` → `index.html` 로 이름 변경 후 업로드
- `audio/` 폴더 생성 후 MP3 220개 전부 업로드
  - GitHub 웹에서: Add file → Upload files → audio/ 폴더째 드래그

### 3. GitHub Pages 활성화
- 저장소 Settings → Pages
- Source: Deploy from a branch
- Branch: main / (root) → Save

### 4. 접속 확인
- 약 1~2분 후 `https://[사용자명].github.io/greek-study/` 접속

### 5. 아이폰/맥북 모두 이 URL로 접속하면 완료!

## 🔊 MP3 매핑 현황 (220개)

| 카테고리 | 파일 수 | 파일명 패턴 |
|---|---|---|
| 알파벳 | 24개 | `alph_*.mp3` |
| 이중모음 | 6개 | `diph_*.mp3` |
| 어휘 동사 | 14개 | `vv1_*.mp3`, `vv2_*.mp3` |
| 어휘 명사 | 12개 | `vn_*.mp3` |
| 어휘 형용사 | 6개 | `va_*.mp3` |
| 현재 능동/수동 변화형 | 12개 | `v_prai_*.mp3`, `v_prmp_*.mp3` |
| 미래 능동/중간/수동 | 18개 | `v_fai_*.mp3`, `v_fmi_*.mp3`, `v_fpi_*.mp3` |
| 미완료 능동/수동 | 12개 | `v_iai_*.mp3`, `v_imp_*.mp3` |
| 단순과거 능동/수동 | 12개 | `v_aai_*.mp3`, `v_api_*.mp3` |
| 현재완료 능동/수동 | 12개 | `v_ppai_*.mp3`, `v_ppmp_*.mp3` |
| 과거완료 능동/수동 | 12개 | `v_pfai_*.mp3`, `v_pfmp_*.mp3` |
| εἰμί 현재 | 6개 | `v_ami_*.mp3` |
| 명사 격변화 | 24개 | `n_logos_*.mp3`, `n_doron_*.mp3`, `n_proph_*.mp3` |
| 정관사 | 22개 | `art_*.mp3` |
| 1·2·3인칭 대명사 | 24개 | `pr1_*.mp3`, `pr2_*.mp3`, `pr3_*.mp3` |

## ⚠️ 주의사항
- audio/ 폴더 경로가 index.html 과 **같은 폴더** 안에 있어야 합니다
- MP3 파일이 없는 단어는 Web TTS(브라우저 기본 음성)로 fallback 됩니다
