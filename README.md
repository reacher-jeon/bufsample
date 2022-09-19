## gRPC  Protocol Buffer file Create Example
**본 자료는 gRPC에 대한 예제로서 protoBuffer 명령어를 직접 사용하는 것이 아닌 Buf.Build 스키마 레지스트리 플랫폼을 이용하였습니다.**

---
## Directory Structure
**현재는 예제 작성을 위해 직관적으로 생성하였지만, 추후 아래의 형식으로 크게는 도메인 그룹 안에 도메인 서비스 -> 마이크로 서비스로 각 서비스 별로 사용되는 
데이터로만 구성 예정**

    │                                        │
    ├─── sample                              ├─── core (Domain Group)
    │   ├─── v1                 --->         │   ├─── Sample(Domain Service) 
    ├─── type (Common)                       │   │   ├─── v1
    │   ├─── 1                               │   │   │   ├─── Sample_One(Micro Service)
    │                           TODO         │   │   │   ├─── Sample_Two(Micro Service)
    │                                        │   │   │   ├─── Sample_Three(Micro Service)
    │                                        │─── Common (Common)
    │                                        │   ├--- v1
    │                           --->         │
    │                                        │
     

---

## Create Command
**아래에 명시된 명령어를 수행 위 디렉토리 구조에 맞게 PB 파일을 생성한다.**

    command : buf generate

---
