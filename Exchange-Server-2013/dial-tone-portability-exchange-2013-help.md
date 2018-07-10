﻿---
title: '발신음 이식성: Exchange 2013 Help'
TOCTitle: 발신음 이식성
ms:assetid: ea62fae0-5e0a-460c-beb6-52532c8c8dbc
ms:mtpsurl: https://technet.microsoft.com/ko-kr/library/Dd876950(v=EXCHG.150)
ms:contentKeyID: 51407763
ms.date: 05/22/2018
mtps_version: v=EXCHG.150
ms.translationtype: MT
---

# 발신음 이식성

 

_**적용 대상:** Exchange Server 2013_

_**마지막으로 수정된 항목:** 2013-01-28_

발신음 이식성을 사용 하면 사서함 데이터베이스, 서버, 또는 전체 사이트에는 영향을 주는 오류에 대 한 제한 된 비즈니스 연속성 솔루션을 제공 하는 Microsoft Exchange Server 2013 의 기능은입니다. 발신음 이식성을 사용 하면 사용자가 원래 사서함 되는 동안 전자 메일을 송수신에 대 한 임시 사서함 복원 또는 복구 합니다. 임시 사서함 동일한 데이터베이스 스키마 버전을 사용 하 여 데이터베이스에는 조직에서 다른 Exchange 2013 사서함 서버에서 동일한 Exchange 2013 사서함 서버에 있을 수 있습니다. 이 더이상 사용할 수 있는 서버에서 이전에 있던 사용자의 사서함을 호스트 하는 대체 서버 수 없습니다. 자동 검색을 지 원하는 클라이언트에 수동으로 사용자의 데스크톱 프로필을 업데이트 하지 않고도 정보가 자동으로 새 서버로 리디렉션됩니다. 사용자의 원래 사서함 데이터를 복원한 후 관리자 단일, 최신 사서함에 사용자의 복구 된 사서함과 사용자의 발신음 사서함 병합할 수 있습니다.

발신음 이식성을 사용 하기 위한 프로세스 *발신음 복구*라고 합니다. 발신음 복구 실패 한 데이터베이스를 교체 하는 사서함 서버에서 빈 데이터베이스를 만드는 단계입니다. *발신음 데이터베이스*라고 하는이 빈 데이터베이스를 실패 한 데이터베이스를 복구 하는 동안 전자 메일 메시지를 주고받을 수 있습니다.

발신음 복구를 수행 하기 위한 다음과 같은 세가지 옵션이 있습니다.

  - **실패 한 데이터베이스를 사용 하 여 서버에서 발신음 복구**   실패 한 데이터베이스를 호스팅하는 서버는 여전히 작동 하는 것이 좋습니다 하는 경우에 해당 서버에서 발신음 복구를 수행 합니다. 이 서버 간에 데이터베이스 파일 이동 하지 않아도 되므로 덜 가동 중지 시간을 의미 합니다. 또한 자동 검색을 지원 하지 않는 클라이언트에 대 한 메시징 프로필을 다시 구성할 필요가 없습니다.

  - **발신음 데이터베이스에 대 한 다른 서버를 사용 하 여 발신음 복구**   서버 실패 하 고 다시 작성 해야 하는 경우, 사용자에 게 기본 메일 기능을 제공 하는 가장 효율적인 방법은 인지를 다른 서버에서 발신음 데이터베이스를 만들고 데이터베이스 이식성을 사용 하 여 사용자의 사서함 구성을 새 서버로 이동 합니다. 원래 (복구 된) 서버에 다시 발신음 데이터베이스를 이동 하는 것이 과정을 하기 때문에 전체 복구 프로세스에 더 많은 시간이 추가 하는이 옵션입니다. 또한이 프로세스는 원본 서버에서 발신음 복구 수행 하는 것 보다 복잡 합니다. 이 프로세스를 수행할 때 발신음 데이터베이스를 호스팅하는 서버에 추가 되는 추가 사용자 로드를 지원 하기 위해 충분 한 리소스가 있어야 합니다. 또한 사용자의 클라이언트에서 자동 검색을 지원 하지 않으면 메시징 프로필에 될 발신음 서버를 가리키도록 다시 구성 해야 합니다.

  - **발신음 복구를 사용 하 여 및 발신음 데이터베이스에 대 한 다른 서버에 유지**   이 비슷합니다 위 옵션을 제외 하 고 다시 원래 서버로 되돌리려면 하지 않습니다. 실패 한 서버를 복구 하려면 불가능 하거나 아니면 없는 경우에는이 옵션을 사용 하는 것이 좋습니다. 이 시나리오에서는 사용자가 일반적으로 서버에 남아는 대체 복구 작업이 완료 된 후. 이 프로세스를 수행할 때 발신음 데이터베이스를 호스팅하는 서버에 추가 되는 추가 사용자 로드를 지원 하기 위해 충분 한 리소스가 있어야 합니다. 또한 사용자의 클라이언트에서 자동 검색을 지원 하지 않으면 메시징 프로필에 될 발신음 서버를 가리키도록 다시 구성 해야 합니다.

세 옵션을 모두 동일한 기본 단계를 수행 합니다.

1.  **실패 한 데이터베이스를 교체 하는 빈 발신음 데이터베이스를 만듭니다.**
    
    이 새 데이터베이스를 보내고 새 메시지를 받을 실패 한 데이터베이스에 있는 사서함을 가진 사용자가 허용 됩니다. 발신음 이식성을 사용 하면 사서함을 이동 하지 않고 다른 데이터베이스에 사용자를 가리킬 수 있습니다. 실패 한 데이터베이스를 보관 하는 서버 이외의 다른 서버에서 발신음 데이터베이스를 만들 경우 새 서버에 사서함 구성 이동 해야 합니다.

2.  **이전 데이터베이스를 복원 합니다.**
    
    실패 한 데이터베이스를 복원 하려면 일반적으로 사용 하는 백업 및 복구 소프트웨어를 사용 합니다. 실패 한 데이터베이스의 백업이 없는 경우 가능한 경우 다른 방법을 사용 하 여 실패 한 데이터베이스를 복구 합니다. 발신음 복구를 위해 동일한 서버를 사용 하는 경우 복구 데이터베이스 (RDB)에 데이터베이스를 복원 해야 합니다.

3.  **복원 된 데이터베이스를 사용 하 여 발신음 데이터베이스를 교체 합니다.**
    
    실패 한 데이터베이스를 복원한 후 발신음 데이터베이스와 교체 합니다. 이렇게 하면 사용자가 보낼 전자 메일을 수신 하 고 복원 된 데이터베이스의 모든 데이터에 액세스 하는 기능입니다. 사용자와 다른 서버에서 발신음 데이터베이스를 이동 된 사서함 구성을 다시 원래 서버로 이동 해야 합니다.

4.  **데이터베이스를 병합 합니다.**
    
    복원 된 데이터베이스에 발신음 데이터베이스에서 데이터를 가져오려면, [New-MailboxRestoreRequest](https://technet.microsoft.com/ko-kr/library/ff829875\(v=exchg.150\)) cmdlet을 사용 하 여 데이터를 병합 합니다.

발신음 복구를 수행 하는 방법에 대 한 자세한 단계 [발신음 복구 수행](perform-a-dial-tone-recovery-exchange-2013-help.md)을 참조 하십시오.
