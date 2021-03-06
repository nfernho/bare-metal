---
copyright:
  years: 1994, 2017
lastupdated: "2017-06-27"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# CPU 속도가 올바르지 않은 이유는 무엇입니까?

CPU 정보를 확인하려고 서버에 로그인한 경우 프로세서의 속도가 올바르지 않을 수 있습니다. 이 불일치는 EIST(Enhanced Intel SpeedStep Technology) 때문일 수 있습니다. EIST는 동적 빈도 스케일링 기술에 대해 Intel에서 사용하는 이름입니다. 이 기술은 다른 시스템에서는 *CPU 스로틀링* 또는 *버스 슬루잉*이라고도 합니다. 일부 AMD 시스템에는 *Cool'N'Quiet* 또는 *PowerNow!*라고 불리는 유사한 기술이 있습니다. 이러한 기술이 모두 동일하지는 않지만 CPU 속도를 느리게 하여 프로세서를 많이 사용하지 않는 경우에 전원 소모 및 열 생성을 줄이려는 동일한 목표를 가지고 있습니다. 서버를 재로드하는 경우 필요에 따라 클럭 속도를 높입니다.

서버의 Intel 프로세서가 SpeedStep 및 고객 포털을 지원하는지 확인하려면 다음을 수행하십시오. 
1. **디바이스**를 클릭하십시오.
* 목록에서 서버를 식별하십시오.
* 서버 이름을 클릭하여 **디바이스 세부사항**을 보십시오.
* **하드웨어**라는 서브섹션을 찾아서 서버의 프로세서 CPU 속도의 모델 번호를 찾으십시오.
* 서버 프로세서 모델 번호를 가지고 [Intel Processor Finder](http://processorfinder.intel.com/)로 이동한 다음 이 번호를 사용하여 프로세서에 대한 더 많은 정보 및 Intel SpeedStep Technology 지원 여부를 찾으십시오.

EIST는 검증된 기술입니다. EIST를 꺼야 할 이유는 없습니다. 그러나 이 기능을 사용하지 않기로 결정한 경우, 지원 팀과 함께 티켓을 열어 이 기능을 사용하지 않도록 설정하십시오. 이 기능을 사용하지 않도록 설정하려면 서버를 다시 부팅해야 합니다.
