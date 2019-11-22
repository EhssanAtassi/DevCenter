---
layout: tutorial
title: 라이브 업데이트를 사용한 기능 토글
weight: 12
show_children: true
---
<!-- NLS_CHARSET=UTF-8 -->
## 라이브 업데이트를 사용한 기능 토글
{: #dab-feature-toggle-live-update }

라이브 업데이트를 사용하여 앱의 다양한 측면을 구성할 수 있으며 원격으로 기능을 켜거나 끌 수 있습니다. 또한 MobileFirst 운영 콘솔에서 직접 변수 값을 변경하여 앱의 특성을 자동으로 제어하십시오.

* **기능**은 앱의 기능을 켜거나 끄는 데 사용되는 on/off 2진 값입니다.
* **특성**은 앱의 작동을 제어하는 데 사용될 수 있는 이름 값 쌍입니다.

>**참고**: 라이브 업데이트는 앱이 준비된 경우에만 사용 가능합니다.

### 라이브 업데이트 사용

다음 방법으로 라이브 업데이트 기능을 사용할 수 있습니다. 

1. **참여**를 선택하십시오. 사용 가능한 서비스의 목록이 표시됩니다.

    ![참여 라이브 업데이트](dab-live-update.png)

2. **라이브 업데이트**를 선택하고 **사용**을 클릭하십시오. 그러면 Mobile Foundation 서버에서 라이브 업데이트가 구성됩니다. 라이브 업데이트 사용 설정에 성공하면 팝업이 표시됩니다.

    ![라이브 업데이트 사용](dab-live-update-enable.png)

3. **+ 새 기능**을 클릭하여 Mobile Foundation 서버에서 새 기능을 정의하십시오. 그러면 아래의 화면이 표시됩니다.

    ![새 특성](dab-live-update-feature-new.png)

4. **기능 ID** 및 **기능 이름**을 입력하고 기본 **가시성**을 설정하십시오.

    * **기능 ID** - 기능의 고유 ID입니다.
    * **기능 이름** - 기능을 설명하는 이름 부여

5. **작성**을 클릭하십시오.

6. 유사하게, 다음 세부사항을 제공하여 라이브 업데이트 특성을 정의하십시오.

    * **특성 ID**
    * **특성 이름**
    * **특성 값**

### 디자인 모드에서 라이브 업데이트에 대한 작업

디자인 모드에서 라이브 업데이트 옵션을 사용으로 설정한 후 선택한 제어의 **텍스트 값** 또는 **텍스트 색상** 또는 **배경색**을 수정하고 새 특성을 정의하여 실시간으로 변경사항을 업데이트하거나 기존 특성을 선택하여 편집할 수 있습니다. 기능 및 연관 특성 목록을 나열하는 라이브 업데이트 테이블에서 특성 값을 수정할 수 있습니다.

#### 제어를 기능에 연관

제어를 기능에 연관하려면 다음을 수행하십시오.

1. 제어를 클릭하여 선택하십시오. 
2. **제어 표시/숨기기** 섹션에서 **기능 선택** 옵션의 **+** 부호를 클릭하여 새 기능을 정의하십시오.  
3. 새 기능의 경우 **기능 ID** 및 **기능 이름**에 값을 제공하고 기능 토글  **켜기/끄기** 스위치를 사용하여 가시성을 사용 또는 사용 안함으로 설정하십시오. 

#### 제어의 특성 수정

제어의 특성을 수정하려면 다음을 수행하십시오.

제어를 선택하고 **${property_name}**을 입력하거나 목록에서 연관시킬 특성을 선택하거나 **새 특성 추가**를 선택하여 새 특성을 작성하고 **특성 ID**, **특성 이름**, **특성 값**에 값을 제공하십시오.
 
라이브 업데이트에서 다음과 같은 제어 및 특성을 사용할 수 있습니다. 

* **단추** - 텍스트 값, 텍스트 색상, 배경색
* **표제** - 텍스트 값, 텍스트 색상
* **레이블** - 텍스트 값, 텍스트 색상

### 코드 모드에서 라이브 업데이트 추가

앱에 라이브 업데이트를 추가하려면 다음을 수행하십시오.

**방법 1**

1. 코드 모드에서 앱을 여십시오.
2. `projectname/ionic/src/app/app.component.ts`로 이동하십시오.

    ![코드 모드에서 라이브 업데이트 추가 - 방법 1](dab-live-update-new-feature-code.png)

3. 라이브 업데이트 방법 초기화로 이동하십시오.
4. 제어의 표시/숨기기를 위한 코드 및 제어의 특성을 설정하기 위한 특성을 편집하십시오.

**방법 2**

1. 코드 모드에서 앱을 여십시오.
2. 코드 스니펫 **</>**로 이동하여 클릭하십시오.
3. **라이브 업데이트**에서 **라이브 업데이트 기능** 또는 **라이브 업데이트 특성** 코드 스니펫을 끌어서 놓으십시오.

    ![코드 모드에서 라이브 업데이트 추가 - 방법 2](dab-live-update-new-feature-code-snippet.png)

4. 제어의 표시/숨기기를 위한 코드 및 제어의 특성을 설정하기 위한 특성을 편집하십시오.