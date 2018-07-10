﻿---
title: '사용자가 음성 메일 대화 내용이 표시 될 수 있도록 허용: Exchange 2013 Help'
TOCTitle: 사용자가 음성 메일 대화 내용이 표시 될 수 있도록 허용
ms:assetid: c5192e05-905c-440f-beec-1f697edc15b3
ms:mtpsurl: https://technet.microsoft.com/ko-kr/library/Ff629381(v=EXCHG.150)
ms:contentKeyID: 51407734
ms.date: 05/22/2018
mtps_version: v=EXCHG.150
ms.translationtype: MT
---

# 사용자가 음성 메일 대화 내용이 표시 될 수 있도록 허용

 

_**적용 대상:** Exchange Online, Exchange Server 2013, Exchange Server 2016_

_**마지막으로 수정된 항목:** 2016-12-09_

음성 메일 미리 보기는에서 UM (통합 메시징)가 음성 메일 메시지를 받을 수 있는 사용자에 게 사용할 수 있는 기능입니다. 음성 메일 미리 보기는 오디오 녹음/녹화의 텍스트 버전을 제공 하 여 기존 UM 음성 메일 기능을 향상 시킵니다. MicrosoftOutlook Web App, Outlook 2010 및 이상 버전, 내 전자 메일 메시지 및 기타 지원 되는 전자 메일 프로그램에서 음성 메일 텍스트가 표시 됩니다. 자세한 내용은 [Microsoft 음성 기술](http://go.microsoft.com/fwlink/p/?linkid=187348)을 참조 하십시오.

## 사용자가 특정 전자 메일 프로그램을 사용할 수 있어야 합니까?

아니요 음성 메일 미리 보기는 모바일 프로그램을 포함 하 여 모든 전자 메일 프로그램의 메시지 본문에 포함 됩니다. 사용자가 다른 전자 메일 프로그램을 사용 하 여 음성 메시지를 받을 수 있는, 있지만 Outlook 및 Outlook Web App 더 나은 경험을 제공 합니다. 예 Outlook 2010 및 그 이후 버전에서 음성 메일 미리 보기 텍스트에서 특정 단어를 클릭할 때 음성 메시지의 오디오 재생 재생을 시작 하는 단어에서 합니다. 음성 메시지의 특정 부분을 수신 대기에 유용 합니다.

## 특정 음성 메일 메시지에 대 한 사용자가 검색할 수 있습니까?

예입니다. 음성 메일 미리 보기 텍스트에서 단어와 구를 자동으로 인덱싱됩니다, 있으므로 음성 메시지 검색 결과에 표시 됩니다. Outlook 2010 및 그 이후 버전 또는 Outlook Web App 에서 사용자가 음성 메시지에 대 한 텍스트를 추가 하려면 **오디오 노트** 상자를 사용도 수 있습니다. 이러한 메모를 쉽게 메시지를 찾을 수 있도록 검색에 포함 됩니다.

## 이 기능을 "음성 메일 미리 보기"를 호출 하는 이유

것은 사용자의 기대를 올바르게 설정 하는 것이 중요 합니다. 음성 메일 미리 보기 같은지 발신자가 음성 메시지에 라고 하는 표시 텍스트를 생성 반드시 하지 않습니다. 사실, 일반적으로 일부 방식으로 정확 하지 않습니다. 할 필요가 없고가 메서드를 호출 하는 것이 좋습니다 더 완벽 한 결과를 보다 일반적으로 구현할 수 있습니다. 미리 보기 제안 판독기 기능의 실제 기능에 더 가깝게 음성 콘텐츠의 요점을 이해할 수 있어야 합니다.

## 음성 메일 미리 보기 텍스트를 더 많이 또는 적게 정확 하 게 만드는 무엇입니까?

이러한 요소를 제어할 수 없는 경우가 종종 및 음성 메일 미리 보기 텍스트의 정확도 따라 요인에 따라 다릅니다. 그러나 음성 메일 미리 보기 텍스트는 경우 보다 정확 하 게 될 가능성이 있습니다.

  - 호출자에 게 의미 속어 용어, 기술 전문 용어 또는 비정상 단어 또는 구를 포함 되지 않은 간단한 음성 메시지를 제공 합니다.

  - 발신자가 음성 메일 시스템에서 쉽게 인식하고 번역하는 언어를 사용합니다. 일반적으로 너무 빠르거나 너무 조용히 말하지 않는 발신자와 어조가 강하지 않은 발신자가 남긴 음성 메시지가 더 정확한 문장과 구문을 생성합니다.

  - 음성 메시지는 배경 소음의 무료 에코, 및 오디오를 삭제 하지 않습니다.

## 언어 음성 메일 미리 보기와 함께 사용할 수 있습니까?

음성 메일 미리 보기 텍스트는 다음 언어로 제공 됩니다.

  - 영어 (미국) (EN-US)

  - 영어(캐나다) - (en-CA)

  - 프랑스어 (프랑스) (FR-FR)

  - 이탈리아어 (IT-IT)

  - 폴란드어(pl-PL)

  - 포르투갈어(포르투갈) - (pt-PT)

  - 스페인어(스페인) - (es-ES)

온-프레미스를 설치한 경우 또는 하이브리드 배포의 UM, UM 언어팩 [Microsoft 다운로드 센터](https://go.microsoft.com/fwlink/?linkid=266542)에서 다운로드할 수 있습니다.

온-프레미스 있는 경우 사용자가 선택한 언어를 사용 하도록 UM 언어팩, 다이얼 플랜 및 자동 전화 교환을 설치한 후 하이브리드 배포를 구성할 수 있습니다. 온라인 고객에 대 한 모든 UM 언어팩을 설치할 필요가 없습니다. 많은 기업이 하나만 UM 다이얼 플랜이 합니다. UM의 기본 언어가 음성 메일 미리 보기를 지 원하는 경우 성공적으로 될 수 있지만 기본 언어로 다이얼 플랜, 음성 메일 미리 보기를 만들려고 시도 합니다. UM 다이얼 플랜을 만들려면 음성 메일 미리 보기 한 언어에서 한번에만 구성할 수 있습니다.

음성 메일 미리 보기 EN-US 이외의 다른 언어로 제공 하는 UM을 구성 하려면 다음이 단계를 따릅니다.

1.  음성 메일 미리 보기를 사용 하려는 언어에서 지원 하는지 확인 합니다.

2.  온-프레미스를 설치한 경우 또는 하이브리드 배포를 다운로드 하 고 적절 한 UM 언어팩을 설치 합니다. 다운로드 하 고 언어팩 설치 다이얼 플랜 기본 언어를 구성 하지 않습니다.

3.  음성 메일 미리 보기에 사용 되는 언어와 다이얼 플랜을 구성 합니다. 자세한 내용은 [다이얼 플랜에 기본 언어 설정](set-the-default-language-on-a-dial-plan-exchange-2013-help.md)을 참조 하십시오.

음성 메일 미리 보기 지원 되는 언어의 텍스트를 표시 하는 방법 전송 된 음성 메시지의 종류에 따라 달라 집니다. 다음과 같은 두가지 유형이 있습니다.

  - **사용자가 자신의 전화로 전화 응답 하지 기록 하는 음성 메시지**
    
    이러한 메시지에 대 한 음성 메일 미리 보기에 사용 되는 언어는 발신자의 음성된 언어 및 언어 지원 여부에 따라 결정 됩니다. 예는 호출자가 음성 메시지를 이탈리아어에서, 리프 이탈리아어 다이얼 플랜에 구성 해 둔 경우 이탈리아어에 음성 메일 미리 보기 텍스트가 나타납니다. 그러나 일본어에서가 남긴 메시지를 발신자를 음성 메일 미리 보기 텍스트가 포함 됩니다 메시지와 함께 하므로 일본어를 사용할 수 없습니다.

  - **Outlook Voice Access 사용자가를 보내는 경우 음성 메시지**
    
    Outlook Voice Access 사용자가 보낸 메시지에 대 한 음성 메일 미리 보기에 사용 되는 언어는 음성 메일 관리자에 의해 제어 됩니다. 따라서, 음성 메일 미리 보기 텍스트 음성 메일 시스템으로 사용 되는 같은 언어에 적용 됩니다. 그러나 음성 메일 미리 보기에 대 한 지원 하지 않는 언어 말하기 발신자 Outlook Voice Access를 사용 하 여 메시지를 남길, 있으면 음성 메일 미리 보기 텍스트가 없는 메시지와 함께 포함 됩니다. Outlook 음성 액세스 하는 방법에 대 한 자세한 내용은, [Outlook Voice Access 설정](setting-up-outlook-voice-access-exchange-2013-help.md)를 참조 하십시오.

## UM을는 음성 메일 미리 보기를 정확 하지 않을 때 인식?

음성 메시지에 포함 된 각 음성 메일 미리 보기에 대 한 신뢰 수준이 결정 됩니다. 음성 메일 시스템을 녹음/녹화에서 소리 단어, 숫자 및 구를 일치 하는 얼마나 잘 측정 합니다. 일치 하는 쉽게, 신뢰도가 높습니다. 높은 수준의 신뢰 더 높은 정확도 일반적으로 연결 됩니다.

특정 값 보다 낮은 신뢰 수준을 확인 하는 경우에 음성 메일 미리 보기 텍스트 위에 **음성 메일 미리 보기 (신뢰도 낮은)** 구가 포함 됩니다. 신뢰도 낮은, 될 음성 메일 미리 보기 텍스트가 정확 하 게 되지 것입니다.

통합된 메시징 음성 인식 ASR (자동)를 사용 하 여 미리 보기에 대 한 해당 신뢰도 계산 하는 있지만 어떤 단어는 잘못 된 하 고 있는 올바른지를 확인할 수 없습니다.

그러나 UM의 음성 메일 미리 보기의 정확 하 게 하는 방법을 알아봅니다 하려고 하는 않습니다. 예 (제공 된 경우) 사용자의 개인 연락처 및 조직의 주소록 또는 소셜 네트워크에서 대화 상대와 발신자의 전화번호를 일치 하도록 시도 합니다. UM을 일치 하는 항목을 발견 하는 경우에 음성 녹음/녹화에 ASR를 실행할 때의 표준 목록의 이름과 단어를 함께 발신자의 이름을 포함 됩니다.

## 음성 메일 미리 보기 사용할 수 없으면 완전히 정확 하 게 있습니까?

너무 신중 하 게, 단어 단위로 미리 보기를 읽고 하려고 하지 하는 경우 사용자를 편리 하 게 음성 메일 미리 보기와 함께 할 수 있습니다. 대신, 이름, 전화번호, 및 통화의 용도 대 한 실마리를 제공할 수 있는 "나에 게 다시 전화" 또는 "논의할 필요"와 같은 구를 찾습니다 해야 있습니다.

음성 메일 미리 보기를 정확 하 게, 메시지를 받아 예상 되지 하지만 사용자는 다음과 같은 질문에 답할 수 있습니다.

  - 이 음성 메시지와 관련 된 내 작업?

  - 이 음성 메시지 기능이 본인에 게 중요 합니까?

  - 발신자 번호를 남길 않은? I 하 여 나열 될 수 있는 번호와에서 다른 입니까?

  - 발신자 고려이 음성 메시지 긴급 한?

  - 이 사용자에 다시 전화 하 모임을 나 가더라도 해야 합니까?

  - 내 요청을 확인 하는 통화를 예상 된 합니다. 확인 통화 입니까?

## 음성 메일 미리 보기 수 설정 또는 해제 설정?

예입니다. 음성 메일 미리 보기를 설정한 경우 사용자 수 켜 또는 Outlook 2010 또는 이후 버전 또는 Outlook Web App 를 사용 하 여 해제 합니다. 그러나 다이얼 플랜 언어 음성 메일 미리 보기를 지원 해야 하 고 해당 언어에 대 한 UM 언어팩을 설치 해야 합니다.

음성 메일 미리 보기 설정을 사용자가 사용 하는 Outlook 2010 또는 이후 버전 또는 Outlook Web App 여부 동일, 하지만 액세스할 수 있게 하 다르게:

**Outlook Web App**

Outlook Web App 에서 음성 메일 미리 보기 설정에 액세스 하려면 사용자가 클릭 **설정** \> **전화** \> **음성 메일**. **음성 메일** 페이지의 설정을 **음성 메일 미리 보기** 에서 사용할 수 있습니다.

사용자가 통합 메시징을 사용 하는 경우 기본적으로 모두 음성 메일 미리 보기 옵션을 사용할 수 있습니다. UM 다이얼 플랜을 음성 메일 미리 보기를 지 원하는 UM 언어팩을 사용 하도록 구성 하는 경우 통합 메시징 만들어집니다 음성 메일 미리 보기 사용자에 대 한 경우:

  - 발신자가 사용자가 전화에 응답 하지 않으면 때문에 음성 메일 메시지를 의미 합니다.

  - UM 사용이 가능한 사용자 Outlook Voice Access에 로그인 하 고 하나 이상의 받는 사람에 게 음성 메시지를 기록 합니다.

구성 요소를 통합 메시징 음성 메시지 및 **받은 음성 메시지를 사용 하 여 미리 보기 텍스트를 포함을** 선택 하는 호출자가 떠난 음성 메일 미리 보기에서 전자 메일 메시지를 만들 때 오디오 파일을 첨부 하 고 받는 사람의 사서함으로 보냅니다. 다이얼 플랜에 구성 된 언어는 음성 메일 미리 보기 지원 포함 되지 않은 경우이 옵션을 해제 하는 것이 좋습니다 하 고 음성 메일 메시지에 포함 된 음성 메일 미리 보기 하지 않으려고 합니다.

사용자가 Outlook 에 로그인 할 때 Voice Access 및은 다른 사용자에 게 음성 메시지를 보내는, **Outlook Voice Access를 통해 보내기 음성 메시지를 사용 하 여 미리 보기 텍스트를 포함** 확인란의 선택을 취소 하려고 할 수도 있습니다. 예, 음성 메일 미리 보기를 지원 하지 않는 언어로 음성 메시지를 보내는 경우 또는 너무 깁니다 때문에 음성 메시지와 함께 음성 메일 미리 보기를 포함 하도록 않을 경우이 작업을 수행 하려는 수 있습니다.
