---
linkTitle: 시작하기
weight: 1
date: '2022-06-07T00:00:00.000Z'
description: >
  클라우드포레는 여러 클라우드 서비스 프로바이더에 분산된 리소스들을 통합하여 체계적으로 관리할 수 있는 서비스입니다. <br> <br>
  가이드를 통해 클라우드포레에 대한 모든 것을 알아보세요. 
title: 시작하기
---

주요 서비스를 이용하기 위해서는 다음 몇 가지 작업이 선행되어야 합니다.

1. [Admin 모드 진입](#1-admin-모드-진입)
2. [도메인 설정](#2-도메인-설정)
3. [워크스페이스 생성 & 사용자 초대](#3-워크스페이스-생성--사용자-초대)
4. [워크스페이스내 프로젝트 생성](#4-워크스페이스내-프로젝트-생성)
5. [서비스 사용 시작 시작하기](#5-서비스-사용-시작하기)

<br>

## 1. Admin 모드 진입

초기에 필요한 설정들은 대부분 Admin 모드에서 이루어집니다. <br>
Admin 역할 타입을 가진 사용자만이 Admin 모드에 접근할 수 있습니다.

![](/guides/admin/admin_mode/admin-mode-01-ko.png)

{{<alert title="💡 Admin 모드란?">}}

* 관리자 전용의 별도 환경으로 분리되어 도메인 내 필요한 여러 주요 설정을 비롯해 Global 데이터 연결, 관리 등이 모두 가능한 모드 입니다.
* Admin을 비롯해 시스템의 권한 체계에 대해서는 [이곳](/ko/docs/guides/permission/)에서 확인할 수 있습니다.

{{</alert>}}

<br><br>

## 2. 도메인 설정

도메인 표시 명을 비롯해 로고, 파비곤(Favicon), 대표 이미지 등을 직접 설정할 수 있습니다.

![](/guides/admin/domain_settings/domain-settings-01-ko.png)![](/guides/admin/domain_settings/domain-settings-02-ko.png)

{{<alert>}}
도메인 설정에 대한 자세한 내용은 [이곳](/ko/docs/guides/admin-mode/domain-settings/)에서 확인할 수 있습니다.
{{</alert>}}

<br>
<br>

## 3. 워크스페이스 생성 & 사용자 초대

데이터 연결, 프로젝트 관리를 위해서는 기본적으로 워크스페이스가 1개 이상 활성화되어 있어야 합니다.

(1) \[관리 > 환경설정 > 워크스페이스]로 이동

(2) 우측 상단 \[+생성] 버튼 클릭

![](/guides/admin/workspaces/workspace-create-workspace-01-ko.png)

(3) 워크스페이스 이름, 설명을 입력하여 쉽고 빠르게 생성 가능

![](/guides/admin/workspaces/workspace-create-workspace-02-ko.png)

(4) 워크스페이스 생성 직후 바로 사용자 초대 가능

* 초대 시 해당 워크스페이스에 특정 역할(=권한)을 필수로 할당하게 됩니다.

![](/guides/admin/workspaces/workspace-create-workspace-04-ko.png)

{{<alert title="💡 사용자 역할(Role)이란?">}}

* Admin 제외 나머지는 특정 워크스페이스에 사용자가 갖는 권한들의 묶음입니다.
* 역할에 대한 자세한 내용은 [이곳](/ko/docs/guides/admin-mode/role/)에서 확인할 수 있습니다.
  {{</alert>}}
  {{<alert>}}
  워크스페이스 생성 및 관리에 대한 자세한 내용은 [이곳](/ko/docs/guides/admin-mode/workspaces/)에서 확인할 수 있습니다.
  {{</alert>}}

<br>

<br>

## 4. 워크스페이스내 프로젝트 생성

(1) 특정 워크스페이스로 이동합니다.

* **워크스페이스 이동 방법 1**: \[관리 > 환경설정 > 워크스페이스]에서 워크스페이스를 선택해서 이동할 수 있습니다.

![](/guides/admin/workspaces/workspace-create-workspace-05-ko.png)![](/guides/admin/workspaces/workspace-create-workspace-06.png)

* **워크스페이스 이동 방법 2**: 우측 상단 \[Admin 모드]를 끄고, 특정 워크스페이스로 이동할 수 있습니다.
  * \[Admin] 모드 끄기
  * 워크스페이스 이동하기

![](/guides/admin/admin_mode/admin-mode-off-ko.png)

![](/guides/admin/workspaces/move-to-workspace-ko.png)

(2) (상단 메뉴)프로젝트로 이동

![](/guides/project/no-project-ko.png)

(3) 우측 상단 \[+생성] 버튼 클릭하여 새 프로젝트 생성

![](/guides/project/project-create-01-ko.png)![](/guides/project/project-create-02-ko.png)

프로젝트의 성향에 따라 '워크스페이스내 전체 사용자'가 접근 가능한 오픈된 프로젝트로,

또는 '초대된 사용자만' 접근 가능한 제한된 프로젝트로 생성할 수 있습니다.

{{<alert>}}
프로젝트 생성 및 관리에 대한 자세한 내용은 [이곳](/ko/docs/guides/project/project/)에서 확인할 수 있습니다.
{{</alert>}}

이제, 서비스 사용을 위한 초기 기본 설정이 끝났습니다.

<br>

## 5. 서비스 사용 시작하기

위의 과정들을 완료한 뒤, 주요 서비스를 좀 더 편리하고 다양하게 이용하고 싶다면 다음 가이드를 참고해주세요.

* [**에셋 인벤토리** 시작하기](/ko/docs/guides/asset-inventory/quick-start)
* [**비용 분석** 시작하기](/ko/docs/guides/cost-explorer/cost-analysis)
* [**얼럿 매니저** 시작하기](/ko/docs/guides/alert-manager/quick-start)
