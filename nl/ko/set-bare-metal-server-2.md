---

copyright:

  years: 2017, 2018
lastupdated: "2018-04-02"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Bare Metal Server 설정
{: #customerportal_setupbaremetal}

Bare Metal Server를 전용 서버로 설정할 수 있습니다.
{:shortdesc}

다음 단계를 사용하여 Bare Metal Server를 설정하십시오.

1. 고유 신임 정보로 {{site.data.keyword.BluSoftlayer_full}} 고객 포털에 로그인하십시오.

2. 메뉴에서 **디바이스** > **디바이스 목록**을 클릭하고 시스템을 찾으십시오. 디바이스 목록에는 모든 디바이스에 대한 자세한 정보가 포함되어 있습니다. 이 목록에서 디바이스를 관리/업그레이드하거나 데이터 사용량 차트를 생성할 수 있습니다.

3. 다음 방법 중 하나로 서버를 관리하도록 선택하십시오.
  * 디바이스 이름 옆의 화살표를 클릭하여 요약을 보고 스냅샷 보기에서 디바이스를 관리하십시오.
  * 서버의 디바이스 이름을 클릭하여 자세한 목록을 보고 디바이스 세부사항 화면에서 디바이스를 관리하십시오.

4. 필요할 때마다 고객 포털에 로그인하지 않고 신속하게 세부사항에 액세스할 수 있도록 서버의 IP 주소와 신임 정보를 안전한 위치에 기록해 두십시오. 개별 디바이스와 계정과 연관된 모든 디바이스의 세부사항을 모두 기록할 수 있습니다.
  * 디바이스 목록에서 개별 디바이스 IP를 보십시오.
  * 디바이스의 스냅샷 보기에서 개별 디바이스 루트 비밀번호를 보십시오.
  * **디바이스 목록**에서 **CSV 다운로드** 옵션을 사용하여 여러 디바이스 IP를 보십시오. 그런 다음 **설정** 톱니바퀴에서 **CSV 다운로드**를 선택하여 전체 디바이스 목록과 세부사항을 스프레드시트 형식으로 다운로드하십시오.

5. 운영 체제 및 기타 소프트웨어에 대한 신임 정보를 업데이트하십시오. 프로비저닝 프로세스 중에 디바이스에 로드된 모든 소프트웨어에는 임시 신임 정보가 지정됩니다. 고객 포털에서 각 디바이스의 비밀번호 탭에서 해당 신임 정보를 보고 관리할 수 있습니다. 이 임시 신임 정보를 사용하여 처음으로 소프트웨어에 액세스한 다음 문자, 숫자 및 기호로 구성된 강력한 비밀번호를 사용하여 소프트웨어의 비밀번호를 변경하십시오. 선택적으로 각 디바이스의 비밀번호 탭에 비밀번호 업데이트를 저장할 수 있습니다. 그러나 고객 포털에 비밀번호를 저장할 때 계정에 액세스할 권한과 적절한 권한이 있는 사용자가 비밀번호 화면에 저장된 비밀번호를 볼 수 있습니다.

6. 사설 네트워크에서 서버에 액세스하십시오. IP를 통한 KVM 및 SSH를 사용하여 원격 데스크탑(RDP)을 통해 디바이스와 상호작용하는 데 {{site.data.keyword.BluSoftlayer_notm}} 인프라 사설 네트워크를 사용할 수 있습니다. 사설 네트워크를 통해 선택한 엔드포인트 또는 가장 가까운 SSL VPN 엔드포인트에 연결하는 데 VPN 액세스 도구를 사용할 수 있습니다. 여러 서비스와 상호작용하는 데도 VPN 액세스가 필요합니다. 사설 네트워크에 액세스하려면 사용자 목록에서 사용자의 VPN 액세스를 편집하십시오. 사용자 목록에 액세스하려면 **계정** > **사용자** > **사용자 목록**을 클릭하십시오. [가상 사설 네트워크 ![외부 링크 아이콘](../icons/launch-glyph.svg)](https://www.softlayer.com/VPN-Access){:new_window} 페이지를 사용하여 다양한 VPN 옵션 중 하나에 연결하십시오.

7. 서버의 상태를 확인하고 스케일링할 시기를 알 수 있도록 모니터링을 설정하십시오. 표준 모니터링 또는 Nimsoft 모니터링 서비스를 사용할 수 있습니다. 고객 포털에서 느린 ping이나 서비스 ping을 사용하여 ping 및 응답 메소드로 표준 또는 기본 모니터링을 사용할 수 있습니다. 고객 포털 또는 세 개의 티어(기본, 고급 및 프리미엄) 중 하나에서 Nimsoft 또는 고급 모니터링도 사용할 수 있습니다.

8. 시스템을 고정하십시오. 사용 가능한 Hardware Firewall을 사용하여 디바이스가 항상 보안되는지 확인하십시오. 규칙이 제대로 확립된 경우 가동 중단 시간 없이 Hardware Firewall을 온디맨드로 프로비저닝하여 원하지 않는 활동으로부터 서버를 보호할 수 있습니다. 방화벽을 주문한 다음 방화벽을 사용하고 규칙을 설정해야 합니다.

9. 디바이스 외부에 안전하게 데이터를 저장하고 데이터가 유실된 경우 다시 로드할 수 있도록 백업을 스케줄링하십시오. 보안 위치에 데이터를 저장하기 위해 다양한 백업 서비스 중에서 선택할 수 있습니다.
  * EVault Backup은 자동화된 에이전트 기반 백업 시스템입니다. "한 번만 설정하면 되는" 인기 디바이스 관리 솔루션입니다. 이 시스템은 Exchange, SQL 등의 Microsoft 소프트웨어와 호환됩니다(추가 플러그인 필요). EVault 사용자는 EVault의 WebCC 웹 기반 애플리케이션을 통해 이 서비스와 상호작용합니다.
  * R1Soft CDP(Continuous Data Protection)는 서버 또는 자체 관리 가상 머신에 설치할 수 있습니다. 단일 인터페이스를 통해 모든 백업을 관리하려는 경우 권장됩니다. 전용 관리 시스템을 통해 R1Soft CDP와 상호작용하므로 가상 머신에 에이전트를 설치할 수 있으며, 추가 기능을 사용할 수 있도록 데이터베이스 플러그인이 제공됩니다.
