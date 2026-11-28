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
- **동화 인물 행진**
  - 호두까기 인형, 생쥐 왕, 별사탕 요정, 눈의 여왕, 성냥팔이 소녀, 진저브레드맨, 스크루지, 말리의 유령, 주석 병정이 트리 둘레를 돕니다. 원작이 퍼블릭 도메인인 인물만 골라 픽셀 그림으로 새로 그렸고, 누르면 이름이 나옵니다.
- **재생목록 편집**
  - 설정(`⚙`)의 `편집`에서 곡을 넣고 빼고(`✓`/`＋`) 순서를 바꿉니다(`▲`/`▼`). 순차·랜덤 재생이 이 목록을 따르며, 목록은 브라우저에 저장됩니다.
- **로우라이트 모드(심야용)**
  - `☾` 버튼이나 설정에서 켜면 화면이 어두운 호박색으로 바뀌고 번쩍임·점멸·불꽃 빈도·음량이 줄어듭니다. `자동`은 22시~7시에만 켜집니다.
- **클릭 / 터치 인터랙션**
  - 화면 어디든 클릭·탭하면 별빛 불꽃과 파동 링이 퍼지며 펜타토닉 오르골 차임이 울립니다.
  - **꼭대기 별 클릭**: 황금 폭죽과 강한 펄스
  - **오너먼트 클릭**: 해당 방울 반짝임 + 같은 색 불꽃
  - **산타 썰매 클릭**: 별가루 폭포 + 썰매 방울 소리
  - **상단 밤하늘 클릭 (산타 대기 중일 때)**: 산타 썰매 즉시 출격!
- **기계식 오르골 캐럴·클래식 14곡 & 화면 꺼짐 방지**
  - 외부 음원 파일 없이 Web Audio API로 **쇠빗(Steel Tine) 비정수배 금속 배음 · 실린더 핀 튕김 클릭 · 우드 울림통 리버브**를 실시간 합성해 영롱한 오르골 음색으로 연주합니다.
  - 박자에 맞춰 트리 전구·오너먼트·꼭대기 별이 반응하며, Screen Wake Lock API로 켜두기 용도를 지원합니다.

---

## 🎵 수록곡 (퍼블릭 도메인 14곡)

모두 저작권이 만료된 곡이며, 녹음을 쓰지 않고 선율을 Web Audio로 직접 합성해 오르골 소리로 연주합니다. 가사나 제목이 종교색이 짙은 곡(참 반가운 성도여, 천사들의 노래가, 천사 찬송하기를, 오 거룩한 밤, 예수 인간 소망의 기쁨)은 기본 목록에서 숨겼습니다(코드에는 `hide:1`로 남아 있음).

### 캐럴·연말 곡
| # | 곡명 | 원곡 / 작곡 |
|---|---|---|
| 1 | **징글벨** (Jingle Bells) | James Lord Pierpont (1857) |
| 2 | **고요한 밤 거룩한 밤** (Silent Night) | Franz Xaver Gruber (1818) |
| 3 | **Deck the Halls** | 웨일스 민요 |
| 4 | **Shchedryk** (종소리 캐럴 선율) | Mykola Leontovych (1916), 본 프로젝트용 편곡 |
| 5 | **올드 랭 사인** (Auld Lang Syne) | 스코틀랜드 민요 |

### 클래식 (주제 부분 발췌)
| # | 곡명 | 작곡 | 선율 출처 |
|---|---|---|---|
| 6 | **꽃의 왈츠** (호두까기 인형) | 차이콥스키 (1892) | webern/mx 저장소의 MusicXML 피아노 악보 |
| 7 | **스케이터 왈츠** (Les Patineurs Op.183) | 발트토이펠 (1882) | GTTM 선율 데이터셋 |
| 8 | **사계 「겨울」 2악장 라르고** | 비발디 (1725) | Mutopia Project (CC BY-SA 3.0) |
| 9 | **할렐루야** (메시아 HWV 56) | 헨델 (1741) | Mutopia Project |
| 10 | **반짝반짝 작은 별 변주곡 주제** (K.265) | 모차르트 (1781) | GTTM 선율 데이터셋 |
| 11 | **트레팍** (호두까기 인형 러시아 춤) | 차이콥스키 (1892) | SBurrell23/Sheets 저장소의 ABC (C장조 편곡) |
| 12 | **환희의 송가** (교향곡 9번) | 베토벤 (1824) | GTTM 선율 데이터셋(앞 8마디) |
| 13 | **아름답고 푸른 도나우** (Op.314) | 요한 슈트라우스 2세 (1867) | Mutopia Project 피아노 편곡 (CC BY-SA 4.0, N. Kouremenos) |
| 14 | **캐논 D장조** | 파헬벨 (약 1700) | Mutopia Project / mfiles (CC BY 3.0) 바이올린 선율, 지속저음은 직접 입력 |

클래식 곡의 화음 반주는 원곡의 베이스·선율에서 자동으로 골라 단순화한 것입니다. 1회 재생이 30초가 안 되던 캐럴 7곡(별사탕 요정의 춤, 그린슬리브스, 저 들 밖에 한밤중에, We Wish You a Merry Christmas, 기쁘다 구주 오셨네, 소나무야, 만백성 기뻐하여라)도 숨겼습니다.

---

## 🚀 사용 방법

### 1. 웹에서 바로 실행 (추천)
브라우저에서 [https://sweetinsam-boop.github.io/xmas-tree/](https://sweetinsam-boop.github.io/xmas-tree/) 를 열고 화면을 탭하면 캐럴이 시작됩니다.  
오른쪽 위 버튼으로 **소리 켜기/끄기(`♪`)**, **재생·타이머 설정(`⚙`)**, **전체 화면(`⛶`)**을 조작할 수 있습니다.
- **설정(`⚙`) 패널**: 14곡 중 원하는 곡 즉시 선택, 재생 순서(`순차` / `랜덤` / `1곡 반복`), 음악 재생 횟수(`무한` / `1·3·6·12곡`), 음악 재생 시간(`무한` / `15분` / `30분` / `1시간` / `2시간`, 끝나면 서서히 줄어들며 멈춤), 트리 애니메이션 지속 시간(`무한` / `10분` / `30분` / `1시간` / `2시간` 슬립 타이머) 지원.

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
