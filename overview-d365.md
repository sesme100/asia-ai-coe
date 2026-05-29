# ASIA - AI CoE 2026

이 환경에서는 Copilot Studio, Copilot for M365 및 Dynamics 365 Suite를 포함한 다양한 기능과 서비스를 살펴볼 수 있습니다. 샌드박스 환경에 대한 자세한 개요는 아래에서 확인할 수 있습니다.

## 샌드박스 환경 정보

   | 제공되는 리소스 | 설정 및 내용 | 상세 설명 |
   | --- | --- | --- |
   | 활성화된 서비스 | `Microsoft Fabric` <br> `기타 Azure 서비스` | 구독에 대한 Owner(소유자) 역할 권한으로 원하는 리소스를 자유롭게 탐색할 수 있습니다 |
   | Azure Entra ID 사용자 | 사전 생성된 Entra ID 사용자 계정 | Entra ID 사용자 계정 1개가 제공됩니다. |
   | Azure 구독 권한 | Azure 구독에 대한 **Owner** 권한 | Azure 구독에 대한 Owner(소유자) 액세스가 제공됩니다. |
   | Azure 크레딧 | **$250 USD** | 그룹당 Azure 사용 한도는 250 USD로 설정됩니다. |
   | 할당된 라이선스 | `Microsoft Copilot Business` <br> `Office 365 apps` <br> `Power Apps Premium` <br> `GitHub Copilot` <br> `Microsoft Copilot Studio User License` <br> `Dynamics 365 Finance` <br> `Dynamics 365 Supply Chain Management` <br> `Dynamics 365 Project Operations` <br> `Dynamics 365 Sales Enterprise Edition` <br> `Dynamics 365 Human Resources` <br> `Dynamics 365 Field Service` <br> `Dynamics 365 Business Central Essentials` <br> `Dynamics 365 Customer Service Enterprise` | 다음 라이선스가 할당되어 사용 가능합니다. |
   | 크레딧 알림 | Azure 크레딧 사용량이 전체의 25%, 50%, 75%, 85%, 90%, 95%, 100%에 도달하면 크레딧 알림이 발송됩니다. | 알림 관련 메일이 수신되었는지 등록된 이메일 받은 편지함을 확인해 주세요. 알림을 통해 Azure 사용량을 미리 파악하고 남은 크레딧을 최적으로 활용할 수 있습니다. |
   | 샌드박스 기간 | 30일/720시간 또는 Azure 소비 크레딧 소진 시 중  먼저 도달하는 시점 | 샌드박스 환경은 30일/720시간 경과 후 또는 Azure 크레딧이 소진된 시점 중 먼저 도달하는 시점에 자동으로 삭제됩니다. |

## 참고 사항:
* Azure 크레딧 사용량에는 샌드박스 환경에서 해커톤 사용을 위해 배포하는 모든 리소스가 포함됩니다.
* Azure 구독에 대한 Owner (소유자) 액세스가 제공됩니다. 필요한 서비스의 기능을 자유롭게 탐색할 수 있으며, 학습 목적으로만 사용하는 것을 권장합니다.
* 각 샌드박스 환경에는 Azure 크레딧에 대한 USD 250의 고정 예산 한도가 있습니다. 샌드박스 환경 이외의 다른 곳에 여기서 제공해드린 리소스를 배포 하시면 안됩니다. 해당 리소스가 할당된 Azure 크레딧을 소비하여 크레딧 한도에 도달하면 환경이 자동으로 삭제될 수 있습니다.

## Microsoft Fabric 비용 최적화

Microsoft Fabric 용량을 배포할 때는 F2 용량을 사용하세요. 대부분의 워크로드에 충분하며, 할당된 Azure 크레딧을 효율적으로 활용하면서 비용을 최적화할 수 있습니다.

## Azure OpenAI 비용 최적화:
Azure OpenAI 서비스는 Standard와 PTU 기반 배포의 두 가지 배포 SKU를 제공합니다. PTU 기반 모델은 강력하지만 **시간당 $2**로 매우 비용이 높습니다. 이 모델을 배포하면 일일 비용이 **$48**에 달해 비용 효율성이 떨어집니다. 또한 PTU 기반 모델을 배포하면 2~3일 내에 크레딧이 소진되어 환경이 자동으로 삭제될 수 있습니다. 따라서 보다 저렴하고 지속 가능한 배포 전략인 **Standard (온디맨드)** 가격 모델을 선택하는 것을 권장합니다.

## 비용 모니터링:
Azure 크레딧 사용량을 모니터링하고 분석하려면 아래 단계에 따라 Azure 구독 페이지로 이동합니다.
+ Azure 포털 홈 페이지에서 검색 창을 사용하여 **구독 (1)** 을 검색하고 결과에서 선택합니다.
  
  ![](media/cost1.png "cost analysis")
  
+ 비용 관리 창에서 비용 분석 탭을 선택합니다. 다양한 서비스 및 리소스와 관련된 비용을 세부적으로 확인할 수 있는 Azure 지출 종합 내역에 액세스할 수 있습니다.

  ![](media/cost2.png "cost analysis")



## 활용 모범 사례:
+ **리소스 사용:** 가상 머신, WebApp, Azure Kubernetes Service, Azure Container Instance 및 기타 리소스를 사용하지 않을 때는 중지하여 Azure 비용을 최소화하세요.
+ **Azure 비용 분석:** 할당된 Azure 구독의 비용 분석 보고서를 정기적으로 확인하여 환경을 장기간 지속 가능한 상태로 유지하세요.
+ **알림 확인:** 알림 관련 메일이 수신되었는지 등록된 이메일 받은 편지함을 확인하세요. 알림을 통해 Azure 사용량을 미리 파악하고 남은 크레딧을 최적으로 활용할 수 있습니다.

## CloudLabs 지원 연락처:
샌드박스 사용관련하여 궁금하신 사항이나 지원이 필요하시다면, 아래와 같이 다음 정보를 제공해 주세요: 

* 샌드박스 사용자 이메일 지원: cloudlabs-support@spektrasystems.com
* 샌드박스 사용자 라이브 채팅 지원: https://cloudlabs.ai/ms-support

지원 문의 시 다음 정보를 제공해 주세요:
+ " **ASIA - AI CoE 2026** 의 참가자 OOO 입니다. 참가 등록 이메일 주소는 `email@contoso.com` (본인 메일 주소) 입니다."라고 입력하시고, 그 후 궁금하신 질문이나 겪고 있는 문제를 작성해 주세요. 
