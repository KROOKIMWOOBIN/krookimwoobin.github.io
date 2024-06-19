---
title: "가상현실실습 기말고사"
excerpt: "동양미래대학교 가상현실실습 기말고사 시험 내용"

categories: [Unity]
tags: [C#, Unity, 2024DongyangMiraeUniversity]

toc: true
toc_sticky: true

date: 2024-06-06 06:17:00 +0800
last_modified_at: 2024-06-06 07:00:00 +0800

pin: false
---
## 문제 형식(17문제)

### 오지선답형 객관식(5점)

### 단답 주관식(10점)

### 서술형 주관식(15점)

## 시험 범위

### Physics와 Collider(충돌)

#### Physics
> 유니티의 물리 엔진은 게임 오브젝트 간의 물리적 상호작용을 시뮬레이션합니다. 물리 엔진은 중력, 충돌, 마찰, 질량 등 다양한 물리적 요소를 고려하여 현실적인 움직임을 구현합니다. 주요 클래스는 Physics이며, Raycast, OverlapSphere 등 다양한 메소드를 통해 물리적 상호작용을 계산할 수 있습니다.

#### Collider
> Collider는 게임 오브젝트가 물리적 상호작용을 감지할 수 있도록 하는 구성 요소입니다. Collider는 여러 종류가 있으며, 각각 다른 용도로 사용됩니다.

| 종류 | 설명 |
| - | - |
| BoxCollider | 직육면체 모양의 콜라이더. |
| SphereCollider | 구형 콜라이더. |
| CapsuleCollider | 캡슐 모양의 콜라이더. |
| MeshCollider | 복잡한 메쉬 형태의 콜라이더. |
| Collider2D | 2D 게임용 콜라이더. |

#### 충돌
> Collider는 Rigidbody와 결합하여 물리적으로 상호작용할 수 있습니다. Rigidbody를 사용하면 게임 오브젝트에 물리 법칙이 적용되어 중력, 이동, 회전 등의 물리 효과를 시뮬레이션할 수 있습니다.

### 사용자 인터페이스(UI)

| 종류 | 설명 |
| - | - |
| Canvas | 모든 UI 요소의 부모 오브젝트로, UI 요소들을 화면에 그리기 위한 공간입니다. |
| Text | 텍스트를 표시하는 데 사용됩니다. |
| Image | 이미지를 표시하는 데 사용됩니다. |
| Button | 클릭 가능한 버튼을 만듭니다. |
| Slider | 슬라이더 바를 만들어 값의 범위를 선택할 수 있습니다. |
| Toggle | 켜짐/꺼짐 상태를 나타내는 토글 버튼입니다. |
| Dropdown | 드롭다운 메뉴를 제공합니다. |

### 컴포넌트

#### AudioSource
> AudioSource는 게임 오브젝트에서 사운드를 재생하는 데 사용됩니다.

#### ParticleSystem
> ParticleSystem은 불꽃, 연기, 물방울 등의 효과를 시뮬레이션하는 데 사용됩니다. 다양한 파티클의 생명 주기, 크기, 색상, 속도 등을 설정할 수 있습니다.

#### Collider
> Collider는 앞서 설명한 대로, 물리적 상호작용을 감지하는 데 사용됩니다. Collider는 게임 오브젝트가 충돌할 수 있는 경계를 정의합니다.

#### Rigidbody
> Rigidbody는 게임 오브젝트에 물리적 속성(질량, 중력, 힘 등)을 부여하여 현실적인 움직임을 시뮬레이션합니다.

#### PyhsicsRaycaster
> PhysicsRaycaster는 UI 요소가 아닌 게임 오브젝트에 대해 레이캐스팅을 수행합니다. 주로 3D 게임에서 마우스 클릭이나 터치 입력을 감지하는 데 사용됩니다.

#### NavMeshAgent
> NavMeshAgent는 유니티의 네비게이션 시스템을 사용하여 게임 오브젝트가 경로를 찾아 이동할 수 있도록 합니다. AI 캐릭터가 장애물을 피해 목적지까지 이동하는 경로를 계산합니다.

### 유니티 애니메이션, 네비게이션

#### 애니메이션
> 유니티의 애니메이션 시스템은 게임 오브젝트의 동작을 애니메이션으로 표현합니다. 애니메이터 컨트롤러를 사용하여 애니메이션 상태를 관리하고, 트리거 및 변수에 따라 상태를 전환할 수 있습니다.

#### 네비게이션
> 유니티의 네비게이션 시스템은 AI 캐릭터가 장면을 탐색할 수 있도록 합니다. NavMesh를 생성하고, NavMeshAgent를 사용하여 경로를 계산합니다. 장애물을 자동으로 피하면서 목적지까지 이동할 수 있습니다.

### 빛(Light) 오브젝트

| 이름 | 설명 |
| - | - |
| Directional Light | 태양광처럼 장면 전체에 빛을 고르게 비춥니다. |
| Point Light | 특정 지점에서 모든 방향으로 빛을 방출합니다. |
| Spot Light | 원뿔 형태로 빛을 방출합니다. |
| Area Light | 사각형 영역에서 빛을 방출합니다. |

### 증강현실(AR) 기술 및 특징
> 증강현실(AR)은 현실 세계에 가상 정보를 겹쳐 보여주는 기술입니다.

| 기술 | 특징 |
| - | - |
| 실시간 상호작용 | 사용자와의 실시간 상호작용을 제공합니다. |
| 현실과 가상의 결합 | 현실 세계의 환경에 가상 객체를 배치하여 상호작용합니다. |
| 감지 기술 | 카메라와 센서를 사용하여 현실 세계를 감지하고 인식합니다. |

### VR 게임 구현화는 과정

1. 프로젝트 설정: 유니티 프로젝트를 생성하고, VR 지원을 활성화합니다.
2. VR SDK 설치: Oculus, SteamVR 등 필요한 VR SDK를 설치합니다.
3. 카메라 설정: VR용 카메라를 설정하고, 플레이어의 시야를 구현합니다.
4. 컨트롤러 설정: VR 컨트롤러를 설정하여 사용자 입력을 처리합니다.
5. 인터랙션 구현: VR 환경 내에서 사용자와의 상호작용을 구현합니다.
6. 성능 최적화: VR의 높은 프레임 속도를 유지하기 위해 최적화를 수행합니다.

### C# Script (클래스, 컴포넌트, 메소드)

#### 클래스
> 클래스는 게임 오브젝트의 동작을 정의합니다. MonoBehaviour를 상속하여 유니티 스크립트를 작성합니다.

```c#
public class PlayerController : MonoBehaviour
{
    void Start()
    {
        // 초기화 코드
    }

    void Update()
    {
        // 매 프레임마다 실행되는 코드
    }
}
```

#### 컴포넌트
> 컴포넌트는 게임 오브젝트에 추가되어 특정 기능을 제공합니다. 예를 들어, Rigidbody, Collider 등이 있습니다.

```c#
public class Example : MonoBehaviour
{
    void Start()
    {
        Rigidbody rb = gameObject.AddComponent<Rigidbody>();
    }
}
```

#### 메소드
> 메소드는 클래스 내에서 특정 작업을 수행하는 함수입니다. 유니티에서는 Start(), Update(), OnCollisionEnter() 등의 메소드가 자주 사용됩니다.

```c#
public class CollisionExample : MonoBehaviour
{
    void OnCollisionEnter(Collision collision)
    {
        Debug.Log("충돌 발생: " + collision.gameObject.name);
    }
}
```