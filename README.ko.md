<div align="center">

# XXD Panel 152｜색면 바탕 페이퍼 아트

일상 사진을 독립적인 아트 포스터로 재연출합니다. 알아볼 수 있는 핵심은 남기고 재료·구도·여백을 다시 설계합니다.

<a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

## 샘플 작품

本项目已发布 8 张实际样片，包含横版与竖版，图片文件位于 `assets/examples/`。

| sample-05 | sample-06 |
| --- | --- |
| ![sample-05](assets/examples/sample-05.png) | ![sample-06](assets/examples/sample-06.png) |
| sample-07 | sample-08 |
| ![sample-07](assets/examples/sample-07.png) | ![sample-08](assets/examples/sample-08.png) |
| sample-09 | sample-10 |
| ![sample-09](assets/examples/sample-09.png) | ![sample-10](assets/examples/sample-10.png) |
| sample-11 | sample-12 |
| ![sample-11](assets/examples/sample-11.png) | ![sample-12](assets/examples/sample-12.png) |

## 잘 맞는 상황과 해결하는 문제

개인 사진 정리, 독립 출판, 전시 습작과 라이프스타일 비주얼에 적합합니다. 평범한 구도, 복잡한 배경, 작은 피사체도 덜어내기·재배열·크롭·크기 변화로 새로운 초점을 만들 수 있습니다. 단순한 사진 필터가 아닙니다.

아래쪽 절반에서는 사진에서 가장 잘 알아볼 수 있는 **피사체, 윤곽, 구조, 자세, 서사적 관계**를 추출하고 새롭게 미술적 판단을 내려 **색면 받침을 둔 페이퍼 아트 콜라주 일러스트**로 재구성합니다. 사진 전체를 복제하거나 사물을 하나하나 옮겨 그리지 마세요. 배경과 무관한 세부 대부분을 적극적으로 삭제하고 원래 대상을 가장 잘 대표하는 시각적 기억의 단서만 남깁니다. 오려낸 종이 윤곽, 종잇조각의 겹침, 기하학적 요약, 약간의 질감을 통해 다시 조직하여 위 사진과의 대응 관계를 한눈에 알아볼 수 있게 합니다.

## 사용 팁

- **선명한 사진 한 장부터 시작하세요:** 피사체, 동작, 관계가 잘 보이는 이미지를 고른 뒤 출력 방식과 비율을 정합니다.
- **파라미터를 한 문장으로 연결하세요:** “상하 / 좌우 / 순수 디자인 + 16:9 / 3:4 / 휴대폰 배경화면”처럼 말하고 컴퓨터·태블릿·스마트워치 크기도 덧붙일 수 있습니다.
- **남겨야 할 것을 분명히 하세요:** 인물, 사물, 동작, 관계, 문구를 지정하되 레이아웃을 지나치게 고정하지 않아야 스타일이 자연스럽게 설계합니다.
- **텍스트 방식을 고르세요:** 이미지에서 지능적으로 생성하게 하거나, `--text exact --copy`로 정확한 문구를 고정하거나, `--text none`으로 글자를 없앨 수 있습니다.
- **사진 영역과 디자인 영역을 설명하세요:** 상하·좌우에서는 사진을 남길 쪽과 다시 디자인할 쪽을 말하고, 순수 디자인·배경화면은 전체 캔버스를 다시 설계한다고 알려 주세요.
- **한 장을 먼저 시험한 뒤 일괄 처리하세요:** 모드, 비율, 텍스트, 언어를 한 장에서 확인하고 같은 설정을 폴더에 적용합니다. 비교를 위해 한 번에 한 변수만 바꾸세요.

## 원본 프롬프트 · 5개 언어

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

중국어 파일은 사용자의 원문을 글자 그대로 보존하며 실행 시 창작과 미적 판단의 유일한 기준입니다. 다른 네 언어는 완전하고 충실한 열람용 번역이며 생성 지시를 다시 쓰지 않습니다.

## 빠른 적합성 확인

원본의 정체성은 유지하면서 구도를 재연출하고, 재료의 특징과 의도적인 여백을 함께 살립니다. 정확한 문구·자동 문구·무문자, 단일 이미지·재귀 폴더 처리 및 아래 네 가지 출력 모드를 지원합니다.

## 네 가지 출력 모드

- `top-bottom`: 전폭 상하 두 영역만 사용합니다. 실제 사진은 위, 디자인은 아래에 정확히 50%씩 둡니다.
- `left-right`: 전고 좌우 두 영역만 사용합니다. 실제 사진은 왼쪽, 디자인은 오른쪽에 정확히 50%씩 두며 상하 구도로 돌리지 않습니다.
- `design-only`: 전체 캔버스에 Panel 152의 디자인 번역만 표시하고 사진은 보이지 않는 참고 자료로 사용합니다.
- `wallpaper-pack`: 휴대폰, iPad, 데스크톱, 시계용 완성 이미지를 각각 만들며 `linked` 또는 `independent`를 선택합니다.

모드와 크기는 여러 개 선택할 수 있습니다. `1:1`, `3:4`, `4:3`, `4:5`, `5:4`, `2:3`, `3:2`, `9:16`, `16:9`, `21:9`, `5:7`, `7:5`, 정확한 픽셀을 지원합니다. 텍스트는 모델 생성, 사용자 원문, 없음 중에서 선택합니다. 폴더 입력은 각 소스를 분리 처리하고 최종 PNG를 하나의 새 작업 폴더에 평면으로 저장합니다.

## 시작하기

```bash
git clone https://github.com/nevertoday/xxd-panel-152.git
npx skills add https://github.com/nevertoday/xxd-panel-152 --skill xxd-panel-152
```

설치 후 Agent 세션을 다시 시작하고 `$xxd-panel-152`을 호출하세요. 사용자 단위 Codex 설치에는 `--global --agent codex --yes`를 추가할 수 있습니다.

```text
/xxd-panel-152 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale ko-KR
/xxd-panel-152 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-152 photo.jpg --mode design-only --size 9:16 --text none
```

전체 실행 계약은 [SKILL.md](SKILL.md), 런타임 어댑터는 [영어](references/xxd-panel-152-prompt.en.md)와 [중국어](references/xxd-panel-152-prompt.zh-CN.md)를 확인하세요.

<!-- xxd-readme-ads:start -->
## XXD 소개

XXD는 Xiaoxiaodong 브랜드 이름의 약자입니다. 이 프로젝트는 [@xiaoxiaodong01](https://x.com/xiaoxiaodong01)이 만들고 관리합니다.

## Xiaoxiaodong 멀티플랫폼 멤버십 · CNY 699/년

> **광고 안내:** 아래 QR 코드와 멤버십·유료 서비스 링크는 XXD의 홍보 정보입니다. 스캔이나 구매는 선택 사항이며 오픈 소스 이용에는 영향을 주지 않습니다.

연간 멤버십 하나로 **Knowledge Planet + XXD 회원 프롬프트 라이브러리 + 모든 General Skills 멤버십**을 함께 이용할 수 있습니다. 각각 따로 구매할 필요가 없습니다.

<!-- xxd-panel-command-system:start -->

### Skills가 함께 작동하는 방식

| 등급 | 포함 내용 | 역할 |
|---|---|---|
| **General** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | 사용 가능한 번호형 Skills를 찾고, 이미지·주제·용도에 맞춰 추천하며, 여러 스타일과 일괄 작업을 정리합니다. |
| **Soldier** | `xxd-panel-NNN` | 각 번호가 고유한 원본 프롬프트와 미학에 따라 General이 배정한 구체적인 작업을 완성합니다. |

<!-- xxd-panel-command-system:end -->

### 회원 혜택

1. **Xiaoxiaodong을 AI 학습 상담자로**
   [Knowledge Planet](https://wx.zsxq.com/group/15554814142882)에서 AI 학습, 도구, 실제 프로젝트에 대해 언제든 질문할 수 있습니다. 답변과 유용한 내용을 회원 자료로 계속 정리합니다.
2. **계속 업데이트되는 회원 프롬프트 라이브러리**
   [XXD 회원 프롬프트 라이브러리](https://vip.xiaoxiaodong.ai/)에는 현재 약 3만 2천 개의 프롬프트가 있으며, 10만 개 이상을 목표로 계속 확장합니다.
3. **모든 General Skills와 사용 지원**
   하나의 멤버십으로 모든 General Skills를 이용하고, 사용 중 도움이 필요할 때 안내와 Q&A를 받을 수 있습니다.
4. **필요성이 높은 요청을 우선 검토**
   회원이 제안한 수요가 높고 꼭 필요한 프롬프트와 Skills는 우선 검토하고 개발합니다.

### 가입 방법

- [회원 웹사이트에서 직접 가입](https://vip.xiaoxiaodong.ai/)할 수 있습니다.
- 또는 아래 QR 코드로 Xiaoxiaodong에게 연락하면 가입을 도와드립니다.

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="Xiaoxiaodong 연락처" width="280"></a></p>
<!-- xxd-readme-ads:end -->

## 라이선스

이 프로젝트(Skill, 프롬프트, 스크립트, 문서, 함께 제공되는 샘플 이미지 포함)는 **PolyForm Noncommercial License 1.0.0**을 따릅니다. 전체 법률 문구는 [LICENSE](LICENSE), 공식 페이지는 <https://polyformproject.org/licenses/noncommercial/1.0.0>에서 확인하세요.

쉽게 말하면 다음과 같습니다.

- 개인은 학습, 연구, 실험, 테스트, 취미 프로젝트, 사적 오락에 사용할 수 있습니다. 자선 단체, 교육 기관, 공공 연구·안전·보건 기관, 환경보호 단체, 정부 기관도 사용할 수 있습니다.
- **비상업적 목적**이라면 사용, 복사, 수정, 파생 작업 제작, 공유가 가능합니다. 공유할 때는 이 라이선스(또는 위 링크)와 저자가 제공한 모든 `Required Notice:` 문구를 함께 제공해야 합니다.
- 상업 제품이나 서비스, 유료 납품, 접근권 또는 라이선스 판매, 상업적 적용으로 이어질 것으로 예상되는 용도에는 사용할 수 없습니다. 상업적으로 사용하려면 저작권자에게 별도의 서면 허가를 받아야 합니다.
- 이 계약은 명시된 저작권 라이선스와 제한된 특허 라이선스만 부여합니다. 상표, 브랜드명 또는 명시되지 않은 다른 권리를 부여하지 않으며 라이선스를 제3자에게 재허여할 수도 없습니다.
- 서면으로 위반 통지를 받으면 32일 안에 준수 상태로 돌아가고 실질적인 시정 조치를 해야 하며, 그렇지 않으면 라이선스가 즉시 종료됩니다. 특허 침해를 서면으로 주장해도 특허 라이선스가 종료됩니다.
- 콘텐츠는 법이 허용하는 범위에서 어떠한 보증도 없이 “있는 그대로” 제공됩니다. 사용에 따른 위험과 잠재적 손실은 사용자가 부담합니다.
