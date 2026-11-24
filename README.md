# 🎄 별빛 캐럴 트리 (Starlight Carol Tree)

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-ffd27a?style=for-the-badge&logo=github)](https://sweetinsam-boop.github.io/xmas-tree/)
[![Single HTML](https://img.shields.io/badge/Zero%20Dependency-Single%20HTML-2fae63?style=for-the-badge)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

PC 모니터·태블릿·스마트폰 화면에 켜두기 좋은 **인터랙티브 크리스마스트리 웹 모션 그래픽**입니다.  
외부 라이브러리나 빌드 없이 **단일 HTML 파일(Canvas 2D + Web Audio)**만으로 동작합니다.

👉 **바로 열기 (설치 불필요)**: https://sweetinsam-boop.github.io/xmas-tree/

![별빛 캐럴 트리 미리보기](preview.png)

---

## ✨ 주요 기능

- **그래픽 → 문자 → ASCII 화면 순환**
  - 24초 장면마다 점·글로우 그래픽 버전과 모든 요소가 문자(`* + ^`, `MERRYCHRISTMAS`, `메리크리스마스`, `NOEL★`, `❄`, `★`)로 그려지는 버전, 화면 전체를 색 문자 격자로 칸칸이 번지듯 바뀌는 ASCII 화면이 차례로 이어집니다.
  - 트리 색도 초록·얼음·장미·보라·황금·무지개로 장면마다 바뀝니다.
- **특별 장면 3종**
  - **불꽃놀이 마을**: 강 건너 마을 위로 트리·산타·루돌프·양말·종·지팡이 사탕·눈꽃 모양과 구·고리·이중·버들·하트·별 불꽃이 터지고 강물에 비칩니다. 하늘을 탭하면 그 자리에서 터집니다.
  - **오로라 캠프**: 오로라와 유성우 아래 텐트와 모닥불, 마지막에 두 유성이 꼭대기 별에서 만납니다.
  - **스노우볼**: 흔들리는 눈 속에서 입자가 모여 눈사람이 만들어집니다.
- **카메라 연출 & 글자 변신**
  - 정면 궤도, 아래서 올려다보기, 위에서 내려다보며 흩어졌다 모이기, `MERRY CHRISTMAS` 글자 변신, 별 클로즈업, 원경 눈 내리는 풍경이 매 바퀴 랜덤 순서로 이어집니다.
- **트리 뒤 먼 하늘을 나는 루돌프 & 산타 썰매**
  - 반짝이는 빨간 코 루돌프와 순록 3마리가 끄는 썰매가 별가루 꼬리를 남기며 트리 뒤 밤하늘을 주기적으로 가로지릅니다. (문자 버전에서도 ASCII 썰매로 전환)
- **입체 눈보라 & 눈 쌓임**
  - 강약 주기와 34초마다 좌우로 부는 돌풍, 회전하는 눈 결정(`❄`), 보케 눈송이, 바닥과 트리 가지에 서서히 쌓이는 눈 효과를 표현합니다.
- **로우라이트 모드(심야용)**
  - `☾` 버튼이나 설정에서 켜면 화면이 어두운 호박색으로 바뀌고 번쩍임·점멸·불꽃 빈도·음량이 줄어듭니다. `자동`은 22시~7시에만 켜집니다.
- **클릭 / 터치 인터랙션**
  - 화면 어디든 클릭·탭하면 별빛 불꽃과 파동 링이 퍼지며 펜타토닉 오르골 차임이 울립니다.
  - **꼭대기 별 클릭**: 황금 폭죽과 강한 펄스
  - **오너먼트 클릭**: 해당 방울 반짝임 + 같은 색 불꽃
  - **산타 썰매 클릭**: 별가루 폭포 + 썰매 방울 소리
  - **상단 밤하늘 클릭 (산타 대기 중일 때)**: 산타 썰매 즉시 출격!
- **기계식 오르골 캐럴 15곡 & 화면 꺼짐 방지**
  - 외부 음원 파일 없이 Web Audio API로 **쇠빗(Steel Tine) 비정수배 금속 배음 · 실린더 핀 튕김 클릭 · 우드 울림통 리버브**를 실시간 합성해 영롱한 오르골 음색으로 연주합니다.
  - 박자에 맞춰 트리 전구·오너먼트·꼭대기 별이 반응하며, Screen Wake Lock API로 켜두기 용도를 지원합니다.

---

## 🎵 수록 오르골 캐럴 (퍼블릭 도메인 15곡)

모든 곡은 저작권이 만료된 퍼블릭 도메인(Public Domain) 명곡으로 구성되어 있으며 순서대로 무한 반복 재생됩니다.

| # | 곡명 | 원곡 / 작곡 | 분위기 |
|---|---|---|---|
| 1 | **징글벨** (Jingle Bells) | James Lord Pierpont (1857) | 경쾌하고 밝은 대표 캐럴 |
| 2 | **별사탕 요정의 춤** (Dance of the Sugar Plum Fairy) | P. I. Tchaikovsky — *호두까기 인형* (1892) | 신비롭고 영롱한 오르골·첼레스타 대표곡 |
| 3 | **고요한 밤 거룩한 밤** (Silent Night) | Franz Xaver Gruber (1818) | 포근하고 잔잔한 6/8박자 아르페지오 |
| 4 | **그린슬리브스** (Greensleeves / What Child Is This?) | 16세기 영국 전통 민요·캐럴 | 아련하고 서정적인 겨울 밤 감성 |
| 5 | **저 들 밖에 한밤중에** (The First Noel) | 영국 전통 캐럴 | 맑고 웅장한 3/4박자 크리스마스 송 |
| 6 | **We Wish You a Merry Christmas** | 16세기 영국 전통 캐럴 | 따뜻하고 축제 같은 피날레 |
| 7 | **Deck the Halls** | 16세기 웨일스 민요 | 흥겨운 4/4박자 |
| 8 | **기쁘다 구주 오셨네** (Joy to the World) | Lowell Mason 편곡 (1839) | 힘차고 밝은 찬가 |
| 9 | **소나무야** (O Tannenbaum) | 독일 민요 | 포근한 3/4박자 |
| 10 | **God Rest Ye Merry, Gentlemen** | 영국 전통 캐럴 | 단조의 고풍스러운 분위기 |
| 11 | **Shchedryk** (종소리 캐럴 선율) | Mykola Leontovych (1916) | 반복 음형이 몰아치는 곡, 본 프로젝트용 편곡 |
| 12 | **참 반가운 성도여** (O Come, All Ye Faithful) | John F. Wade (18세기) | 장엄한 찬가 |
| 13 | **천사들의 노래가** (Angels We Have Heard on High) | 프랑스 전통 캐럴 | 긴 글로리아 선율 |
| 14 | **천사 찬송하기를** (Hark! The Herald Angels Sing) | Felix Mendelssohn (1840) | 웅장한 합창곡 |
| 15 | **올드 랭 사인** (Auld Lang Syne) | 스코틀랜드 민요 | 한 해를 마무리하는 곡 |

---

## 🚀 사용 방법

### 1. 웹에서 바로 실행 (추천)
브라우저에서 [https://sweetinsam-boop.github.io/xmas-tree/](https://sweetinsam-boop.github.io/xmas-tree/) 를 열고 화면을 탭하면 캐럴이 시작됩니다.  
오른쪽 위 버튼으로 **소리 켜기/끄기(`♪`)**, **재생·타이머 설정(`⚙`)**, **전체 화면(`⛶`)**을 조작할 수 있습니다.
- **설정(`⚙`) 패널**: 15곡 중 원하는 곡 즉시 선택, 재생 순서(`순차` / `랜덤` / `1곡 반복`), 음악 재생 횟수(`무한` / `1·3·6·12곡`), 트리 애니메이션 지속 시간(`무한` / `10분` / `30분` / `1시간` / `2시간` 슬립 타이머) 지원.

### 2. 로컬에서 실행
저장소를 내려받은 뒤 `index.html`을 브라우저로 열면 바로 실행됩니다.

```bash
git clone https://github.com/sweetinsam-boop/xmas-tree.git
open xmas-tree/index.html
```

---

## 🛠 기술 스택

- **HTML5 Canvas 2D**: 3D 원근 투영, 가산 합성(`lighter`), 오프스크린 스프라이트 캐시
- **Web Audio API**: 실시간 오실레이터·노이즈 합성 캐럴 + 클릭 차임벨 (iOS 무음 모드 대응 `audioSession.type = 'playback'`)
- **Zero Dependencies**: 외부 JS/CSS 번들러나 프레임워크 없음 (Google Fonts만 선택 로드)

---

## 🌍 English Summary

**Starlight Carol Tree** is a zero-dependency, single-file interactive Christmas tree screensaver built with HTML5 Canvas 2D and Web Audio API.

- **Live Demo**: https://sweetinsam-boop.github.io/xmas-tree/
- **Highlights**: Seamless morphing between particle graphics and ASCII text mode, 6 cinematic camera scenes (`MERRY CHRISTMAS` morphing included), flying Santa & Rudolph sleigh across the distant sky, dynamic snowstorm & accumulation, interactive click/tap starbursts & chimes, and a realistic **Web Audio Music Box (steel tine overtones + wood reverb)** playing 6 public-domain Christmas classics (*Jingle Bells*, *Dance of the Sugar Plum Fairy*, *Silent Night*, *Greensleeves*, *The First Noel*, *We Wish You a Merry Christmas*).

## 📄 License

MIT License — 자유롭게 사용, 수정, 공유할 수 있습니다.
