작동 테스트
===============================================

.. raw:: html

   <div class="video-wrap">
      <iframe width="700" height="394" src="https://www.youtube.com/embed/gJar8GA4ik4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
   </div>


| ※영상의 내용이 초기 버전을 기준으로 촬영되었기 때문에 참고만 해주시고, 작업은 매뉴얼을 따라 진행해주세요.


.. raw:: html

    <style> 
    .orangecircle {color:#ff5300; font-size:20px} 
    .blackcircle {color:black; font-size:20px} 
    .bluecircle {color:#3172f4; font-size:20px}
    .skybluecircle {color:#00FFFF; font-size:20px}
    .yellowcircle {color:#fbbc05; font-size:20px}
    .subtitle {color:black; font-weight:bold; font-size:28px}
    .blackbold {color:black; font-weight:bold;}
    .redbold {color:red; font-weight:bold;}
    </style>

.. role:: orangecircle
.. role:: blackcircle
.. role:: bluecircle
.. role:: skybluecircle
.. role:: yellowcircle
.. role:: subtitle
.. role:: blackbold
.. role:: redbold

|
| ※작동테스트 과정은 3D 프린터가 조립이 잘되었는지 필요한 기능들을 작동시켜 보는 과정입니다.
| 순서대로 차근차근 진행해주시기 바랍니다.



전원 연결
--------------------------

|
| :subtitle:`Step.1`

.. image:: /images/WorkingTest/step_1.jpg
   :width: 800

| :blackcircle:`●` 검정색 전원 케이블을 찾아줍니다.

|
| :subtitle:`Step.2`

.. image:: /images/WorkingTest/step_2.jpg
   :width: 800

| :orangecircle:`●` 전원 케이블을 SMPS 파워 아래 전원 커넥터에 연결합니다.
| :blackcircle:`●` 연결 후 전원 플러그를 끼우고, 전원 스위치를 켭니다.
| ※ 전원이 켜지지 않는 다면, :ref:`전원이 켜지지 않는 경우 <targetCannotOnPrinter>` 항목을 확인하세요.
| ※ 전원이 켜지면, "베드 레벨링 값을 불러올 수 없습니다." 에러가 뜰텐데, 조립 후 레벨링 작업이 안되어 있으면 안내되기 때문에, 신경쓰지 않으셔도 됩니다.

|

원점 이동(Home) 점검
--------------------------

|
| :subtitle:`Step.3`

.. image:: /images/WorkingTest/step_3.jpg
   :width: 800

| :blackcircle:`●` 전원을 켜면, 디스플레이도 켜집니다. 첫 화면은 메인화면이라 부릅니다.
| :blackcircle:`●` 화면의 상태 값과 로고 이미지 등이 깨진 것이 있는지 확인합니다.
| :blackcircle:`●` 표시된 상태 값은 예시입니다. 상태 값 설명은 매뉴얼 뒷부분에 설명합니다.

|
| :subtitle:`Step.4`

.. image:: /images/WorkingTest/step_4.jpg
   :width: 800

| :orangecircle:`●` 메인 화면에서 메뉴(1) 버튼을 선택합니다.
| :orangecircle:`●` 이후 나타나는 여러 메뉴 중 '이동'(2) 버튼을 선택합니다.

|
| :subtitle:`Step.5`

.. image:: /images/WorkingTest/step_5.jpg
   :width: 800

| :orangecircle:`●` 이어 'Home'(1)와 'X'(2) 버튼을 누르고, 작동하는 모습을 확인합니다.
| :blackcircle:`●`  Auto home이라는 기능로도 불리며, 원점으로 이동하는 기능으로 자주 사용됩니다.
| ※ 예열을 권장하지만, 조립 후 첫 작동이기 때문에 예열은 하지 않아도 됩니다.

|
| :subtitle:`Step.6`

.. image:: /images/WorkingTest/step_6.png
   :width: 600
   :align: center

|
| :bluecircle:`●` 익스트루더가 왼쪽 끝까지 도달하는지 확인합니다. 도달한다면 Step.7을 진행합니다.
| :blackcircle:`●` 도달하지 않는 경우, 손으로 왼쪽 끝까지 밀어봅니다. 
| -손으로 밀었을 때, 뻑뻑함이 느껴지거나 끝까지 도달하지 못하면, 도금봉의 마찰이나, 
| 벨트 텐션에 의한 마찰일 가능성이 있습니다. 도금봉에 구리스를 발라주고, 벨트 텐션을 
| 살짝 풀어줍니다. :ref:`(X 텐션 조정) <targetAssem3_Step36_X_Tension>`
| -손으로 밀었을 경우 끝까지 도달한다면, 모터 감도를 조절해봅니다. :ref:`(세부조정-모터감도) <targetMotorSensitivity>`
| -작동시 움직임이 미동도 없을 정도면, :ref:`모터가 움직이지 않는 경우 <targetNotWorkingStepper>` 를 확인해보세요. 

|
| :subtitle:`Step.7`

.. image:: /images/WorkingTest/step_7.jpg
   :width: 800

| :orangecircle:`●` 이어 'Y'(1) 버튼을 누르고, 작동하는 모습을 확인합니다.

|
| :subtitle:`Step.8`

.. image:: /images/WorkingTest/step_8.png
   :width: 600
   :align: center

|
| :bluecircle:`●` 베드가 뒷쪽 끝까지 도달하는지 확인합니다. 도달한다면 Step.9을 진행합니다.
| :blackcircle:`●` 도달하지 않는 경우, 손으로 뒷쪽 끝까지 밀어봅니다. 
| -손으로 밀었을 때, 뻑뻑함이 느껴지거나 끝까지 도달하지 못하면, 도금봉의 마찰이나,
| 벨트 텐션에 의한 마찰일 가능성이 있습니다. 도금봉에 구리스를 발라주고, 벨트 텐션을 
| 살짝 풀어줍니다. :ref:`(Y 텐션 조정) <targetAssem2_Step15_Y_Tension>`
| -손으로 밀었을 경우 끝까지 도달한다면, 모터 감도를 조절해봅니다. :ref:`(세부조정-모터감도) <targetMotorSensitivity>`
| -작동시 움직임이 미동도 없을 정도면, :ref:`모터가 움직이지 않는 경우 <targetNotWorkingStepper>` 를 확인해보세요. 

|
| :subtitle:`Step.9`

.. image:: /images/WorkingTest/step_9.jpg
   :width: 800

| :orangecircle:`●` 이어 'Z'(1) 버튼을 누르고, 작동하는 모습을 확인합니다.

|
| :subtitle:`Step.10`

.. image:: /images/WorkingTest/step_10.png
   :width: 600
   :align: center

|
| :bluecircle:`●` 익스트루더와 베드가 중앙으로 위치하며, Z축 방향으로 내려와서 멈춘다면 다음을 진행합니다.
| :blackcircle:`●` :blackbold:`"원점이동 실패, 재부팅 필요"` 에러나타날 수 있습니다. 이 에러는 두 가지 경우에 나타납니다. 
| :ref:`원점이동 실패 에러 원인 확인하기 <targetFailedHoming>`
| ※ X,Y,Z을 연속으로 실행하는 버튼이 Home 버튼입니다.
| ※ Z Home 이 완료되었을 때, 노즐이 정중앙에 위치하는 것이 아니라 중앙에서 살짝 왼쪽 앞에 위치하는 것은 정상적인 작동입니다.
| ※ Z Home 시 하강하지 않고 상승만 하다 끝나는 경우, 레벨링 센서의 :ref:`배선 <targetWiringTotal>` 과 :ref:`작동상태 <targetFailedHoming>` 를 확인해보세요.

.. _targetWorkingTest_SensorHeight:

^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: /images/WorkingTest/41_Sensor_Height.png
   :width: 600
   :align: center

| 마지막으로 센서의 높이를 확인합니다. 레벨링 센서는 노즐보다 약간 위에 있어야 좋습니다. 그렇다고 너무 높게도 안됩니다. 레벨링 센서가 너무 높으면, 정상적인 Home 을 할 수 없으며, 레벨링 센서가 노즐보다 낮으면, 레벨링을 제대로 진행할 수 없습니다.

|
| :subtitle:`※구리스 바르기`

.. image:: /images/WorkingTest/step_10_additional_1.jpg
   :width: 800

| :blackcircle:`●` 구리스는 사진과 같이 흰색 통에 담겨 있으며, 부속품과 함께 동봉되어 있습니다.
| :blackcircle:`●` 나무젓가락, 막대를 이용하여, 약간 덜어낸 다음, 리드스크류에 발라줍니다.

|

.. image:: /images/WorkingTest/step_10_additional_2.jpg
   :width: 800

| :bluecircle:`●` 리드스크류의 왼편, 오른편 모두 얇게 발라줍니다.


|

팬 점검
--------------------------

|
| :subtitle:`Step.11`

.. image:: /images/WorkingTest/step_11.jpg
   :width: 800

| :orangecircle:`●` 메인 화면에서 메뉴(1) 버튼을 선택합니다.
| :orangecircle:`●` 이후 나타나는 여러 메뉴 중 '준비/점검'(2) 버튼을 선택합니다.
| :blackcircle:`●` '준비/점검' 메뉴는 준비, 프린터 점검을 하는 메뉴들로 구성되어 있습니다.

|
| :subtitle:`Step.12`

.. image:: /images/WorkingTest/step_12.jpg
   :width: 800

| :orangecircle:`●` 첫 번째 점검인 '팬 점검'(1) 버튼을 누릅니다.
| :blackcircle:`●` 메인팬 작동을 확인합니다.(V2에서 메인팬은 대기중에 작동하지 않습니다.)
| :blackcircle:`●` 작동하지 않으면 취소 버튼을 누르고 배선을 점검합니다.

|
| :subtitle:`Step.13`

.. image:: /images/WorkingTest/step_13.jpg
   :width: 800

| :blackcircle:`●` 다음은 보조팬을 테스트합니다. 보조팬이 작동하는지 확인합니다.
| :blackcircle:`●` 작동하지 않으면 취소 버튼을 누르고 배선을 점검합니다.
| :blackcircle:`●` 보조팬 테스트 중에는 메인팬은 작동하지 않습니다.

|
| ※ 익스트루더의 보조팬이 사진처럼 덕트에 끼워져 있는지 확인합니다. 살짝 들려서 배송될 수 있기 때문에, 테스트 중에 보조팬을 덕트에 끼워줍니다.

.. image:: /images/WorkingTest/Extruder_SubFan.png
   :width: 600
   :align: center

|

예열 점검
--------------------------

|
| :subtitle:`Step.14`

.. image:: /images/WorkingTest/step_14.jpg
   :width: 800

| :orangecircle:`●` 이어서 두 번째 점검인 '예열'(1) 버튼을 누릅니다.
| :blackcircle:`●` 누르게 되면 예열이 시작됩니다. 온도와 경과시간은 '확인' 버튼을 눌러야 표시됩니다.

|
| :subtitle:`Step.15`

.. image:: /images/WorkingTest/step_15.jpg
   :width: 800

| :blackcircle:`●` 노즐 예열이 완료되면, 자동으로 베드 예열로 넘어갑니다.
| :blackcircle:`●` 온도와 경과시간은 '확인' 버튼을 눌러야 표시됩니다.

|
| :subtitle:`Step.16`

.. image:: /images/WorkingTest/step_16.jpg
   :width: 800

| :blackcircle:`●` 예열 테스트가 끝나면 결과를 알려줍니다.
| :blackcircle:`●` 노즐은 3분 이상, 베드는 5분 이상 소요되면, 테스트 완료되지 않습니다.
| :blackcircle:`●` 확인을 누르고 다음 테스트를 준비합니다.

|

XY 점검
--------------------------

|
| :subtitle:`Step.17`

.. image:: /images/WorkingTest/step_17.jpg
   :width: 800

| :orangecircle:`●` 3D 프린터 위에 놓인 물건이 없는지 확인 후, 'XY 점검'(1) 버튼을 누릅니다. 
| :blackcircle:`●` 따로 팝업창이 뜨지 않으며, 바로 X,Y의 동작 테스트가 진행됩니다.
| :blackcircle:`●` X,Y값이 표시되면 X,Y의 배선, 벨트 텐션이 정상 범위에 있음을 뜻합니다. 에러없이 테스트가 완료되었으면 :ref:`Step.20 <targetStep20InWT to paragraph>` 을 진행합니다.

|
| :subtitle:`Step.18`

.. image:: /images/WorkingTest/step_18.jpg
   :width: 800

.. image:: /images/WorkingTest/step_18_2.png
   :width: 800

| :blackcircle:`●` 만일 벨트 장력이 약하다면 해당, 축의 벨트가 약하다고 표시됩니다.
| :blackcircle:`●` 벨트 장력을 조절하고 다시 테스트합니다.
| :blackcircle:`●` 또한, X축 모터 감도 조절이 필요하다고 알림이 나타날 수 있습니다.
| :blackcircle:`●` 메뉴 - 세부조정에서 모터 감도를 조절해 줍니다. :ref:`(세부조정-모터감도) <targetMotorSensitivity>`

|
| :subtitle:`Step.19`

.. image:: /images/WorkingTest/step_19.jpg
   :width: 800

| :blackcircle:`●` X, Y모터가 배선이 잘못된 경우라면, 잘못된 배선을 감지하여, 알려줍니다.
| :blackcircle:`●` X, Y모터의 배선을 다시 한번 더 점검합니다.


|

.. _targetStep20InWT to paragraph:

필라멘트 점검
--------------------------

|
| :subtitle:`Step.20`

.. image:: /images/WorkingTest/step_20.jpg
   :width: 800

| :orangecircle:`●` 다음 점검으로 '필라멘트'(1) 버튼을 누릅니다
| :blackcircle:`●` 이번 점검은 예열이 필요한 상황이므로, 예열이 안되었다면, 예열하라는 경고 문구가 뜹니다. 예열 완료 후 다시 '필라멘트'(1) 버튼을 눌러줍니다.

|
| :subtitle:`Step.21`

.. image:: /images/WorkingTest/step_21.jpg
   :width: 800

.. image:: /images/WorkingTest/step_21_1.png
   :width: 600

| :blackcircle:`●` 익스트루더의 스프링을 임시로 19~20mm길이 만큼 조여줍니다.
| :blackcircle:`●` 이 범위는 권장 범위로 조립상태에 따라 범위를 벗어날 수 있습니다.
| :blackcircle:`●` ※ 와셔를 제외한 스프링만의 길이입니다.

|
| :subtitle:`Step.22`

.. image:: /images/WorkingTest/step_22.jpg
   :width: 800

| :blackcircle:`●` 필라멘트를 삽입하기 위해서 끝부분을 뾰족하게 2번 잘라줍니다.
| ※ 필라멘트가 많이 휘어있다면, 삽입이 안될 수 있으니 곧게 펴줍니다.
| :blackcircle:`●` 잘라준 뒤 삽입합니다. 삽입 후, 확인 버튼을 누릅니다.
| ※ 필라멘트가 삽입되지 않는다면, :ref:`필라멘트가 삽입되지 않는 경우 <targetCannotInsertFila>` 항목을 참고하세요.

|
| :subtitle:`Step.23`


.. image:: /images/WorkingTest/step_23.png
   :width: 600
   :align: center
   
.. image:: /images/WorkingTest/Printer_41cm.png
   :width: 400
   :align: center

| :blackcircle:`●` 필라멘트가 삽입되면서 토출되는 것을 확인합니다.
| :blackcircle:`●` 필라멘트가 토출되는 길이는 40~45cm 이상이어야 좋습니다.
| :blackcircle:`●` 프린터의 하단 옆면의 길이가 약 41cm 이기 때문에 이와 비교하세요.
| :blackcircle:`●` 토출된 필라멘트 길이가 짧지 않다면, 다음 과정인 :ref:`레벨링 <targetLeveling to paragraph>` 으로 넘어갑니다.
|
| ※토출 길이가 40cm 보다 짧고, 감지된 횟수가 많은 경우에는 아래를 진행해줍니다.
| :blackcircle:`●` 메인 펌웨어 버전 1.2 기준으로 토출 길이가 40cm 이며, 버전을 확인해줍니다. (메뉴-설정-정보에서 확인)
| :blackcircle:`●` 예열을 하고 충분히 시간이 지난 뒤(10분 정도) 다시 시도해 봅니다.
| :blackcircle:`●` 익스트루더 앞부분 스프링을 먼저 살짝 풀고 다시 시도해봅니다. 이 과정에서 스프링의 길이가 20mm 를 약간 넘어가도 무방합니다.
| :blackcircle:`●` 익스트루더 앞부분 스프링을 완전 풀고, 내부에 이물질이나 찌꺼기가 있는지 확인합니다.
|

.. image:: /images/WorkingTest/Extruder_Filament_Path.png
   :width: 800

.. raw:: html

   <center-text-for-figure>익스트루더 내부(왼)와 필라멘트가 삽입된 모습(오)</center-text-for-figure>

| 
| ※ 필라멘트가 토출되지 않는다면, 위 사진 처럼 익스트루더 정면의 스프링을 끝까지 풀어서 내부를 한번 살펴보시기 바랍니다.
| 필라멘트가 경로로 삽입이 잘 되도록, 뾰족하게 잘라주시고 곧게 펴주시기 바랍니다.

|

레벨링이란?
--------------------------

.. _targetLeveling to paragraph:

| 레벨링은 노즐과 베드 사이의 간격을 조절하는 과정입니다. 메탈 V2 같은 경우 오토레벨링이 적용되어 있습니다. 오토레벨링이라 하더라도 초반의 약간의 설정이 필요합니다. 오토레벨링을 설정하는 순서는 크게 좌우 수평 맞추기, 실시간 레벨링 보정이 있습니다. 

.. image:: /images/WorkingTest/leveling_1.jpg
   :width: 800

|  조립과정에서 좌우의 수평이 맞지 않은 경우가 있을 수 있습니다. 이런 경우 오토레벨링이 적용된다 하더라도 특정 부분에서 레벨링이 약간씩 안 맞을 가능성이 있습니다. 이런 경우를 막기 위해 좌우 수평을 조절해야 합니다. 위의 그림은 이해를 돕기 위해 과장된 것입니다. 이를 조정하는 과정은 :ref:`Step.24 <targetStep24InWT to paragraph>` 에 설명되어 있습니다.

.. image:: /images/WorkingTest/leveling_2.jpg
   :width: 800

| 오토레벨링이 적용된 경우, Z축으로 원점 설정(Auto home)을 하면 대부분 노즐이 베드에 닿지 않습니다. 그림과 같은 모습입니다. Z축 원점설정을 하였는데 보드가 프로그램 상에서 인식하는 원점이랑 실제의 원점이랑 같지 않다면, 출력을 하더라도 허공에서 출력하거나, 잘못된 높이에서 출력할 가능성이 높습니다. 이러한 상황에서 노즐과 베드 사이의 간격을 조절해 주기 위한 값이 'Z 프로브 오프셋'입니다.
|
| 조절하는 방법은 실제로 출력 테스트를 하면서 적당한 값을 찾고 저장하는 것입니다.( :ref:`Step.28 <targetStep24InWT to paragraph>` 에서 상세 설명) 이렇게 좌우 수평과, 레벨링 보정까지 마치게 되면, 레벨링이 완료되게 됩니다.

| ※ 필라멘트가 삽입된 상태에서 예열을 하고 레벨링을 진행하는 것을 권장드립니다.

|

Z수평조절
--------------------------

.. _targetStep24InWT to paragraph:

|
| :subtitle:`Step.24`

.. image:: /images/WorkingTest/step_24.jpg
   :width: 800

| :orangecircle:`●` 다음 점검으로 'Z수평조절'(1) 버튼을 누릅니다.

|
| :subtitle:`Step.25`

.. image:: /images/WorkingTest/step_25.jpg
   :width: 800

| :blackcircle:`●` 첫 번째로 X의 좌우 수평을 맞추기 위해 Z축이 상승하고 내려옵니다.
| :blackcircle:`●` 내려오면, 히트베드의 꼭지점의 높이를 측정하고 화면에 표시합니다.
| :blackcircle:`●` 다음 과정을 통해 베드의 각 꼭지점 높이를 유사하게 맞추어야 됩니다.

|
| :subtitle:`Step.26`

.. image:: /images/WorkingTest/step_26.jpg
   :width: 800

| :blackcircle:`●` 맞추고자 하는 부분을 정합니다. (가장 오차가 큰  베드 왼쪽 앞 2번을 예시로 합니다.)
| :orangecircle:`●` 사진과 같이 나비너트를 돌려줍니다. (반시계=값 증가, 시계=값 감소)
| :bluecircle:`●` 나비너트를 조절하고, 화면의 2번 부분을 터치하여 값을 확인합니다.

|
| :subtitle:`Step.27`

.. image:: /images/WorkingTest/step_27.jpg
   :width: 800

| :blackcircle:`●` 베드의 4군데의 값이 비슷해졌다면, '뒤로' 버튼을 눌러 다음을 준비합니다.
| :blackcircle:`●` 완료 후 실제 눈으로도 비틀어진 부분이나 수평이 맞는지 확인합니다.
| :blackcircle:`●` 4군데 값이 아주 비슷할 필요는 없으며, 0.1 단위 까지만 맞추면 됩니다.

| ※ 하강 과정시 원점이동 실패라는 문구가 뜨면, :ref:`원점이동 실패의 대처 방법 <targetFailedHoming>` 을 확인하세요.

|

.. _targetStep28InWT to paragraph:

레벨링
--------------------------

| 레벨링의 목적은 적절한 높이를 맞춰주는 데에 있습니다.
| 레벨링이 맞지 않으면 안착이 안되어 출력 실패로 이어질 수 있습니다.
| 이 부분이 초보자분들이 헤멜 수 있습니다만 잘 따라오시기만 하면 문제 없으실 겁니다.

.. image:: /images/WorkingTest/leveling_gap.gif
   :width: 600

| 베드와 노즐간의 높이가 너무 높으면, 안착이 안되고 필라멘트가 노즐 주변에 붙습니다.
| 반대로 높이가 낮으면, 필라멘트가 퍼지거나, 베드에 긁힘이 발생합니다.
| 다음 과정을 통해 높이를 맞춰보세요.

|
| :subtitle:`Step.28`

.. image:: /images/WorkingTest/step_28.jpg
   :width: 800

| :orangecircle:`●` 다음 점검으로 '레벨링'(1) 버튼을 누릅니다.
| :blackcircle:`●` 이번 점검은 예열이 필요한 상황이므로, 예열이 안되었다면, 예열하라는 경고 문구가 뜹니다. 예열 완료 후 다시 '레벨링' 버튼을 눌러줍니다.

|
| :subtitle:`Step.29`

.. image:: /images/WorkingTest/step_29.jpg
   :width: 800

.. image:: /images/WorkingTest/step_29_2.gif
   :width: 800

| :blackcircle:`●` 레벨링이 시작되면, 원점이동(auto home) 과정 이후 출력이 진행됩니다.
| :blackcircle:`●` 왼쪽 앞에서 시작해서 지그재그로 움직인 뒤, 왼쪽 뒤에서 끝납니다.
| :blackcircle:`●` 진행 도중에 조그 버튼을 이용하여, 높이(베드와 노즐간격)를 실시간으로 조절해야 합니다.
| :blackcircle:`●` Step.30을 참고하여, 레벨링 도중에 높이를 조절해 주셔야 적절한 높이를 맞출 수 있습니다.
| ※원점이동(auto home) : xyz의 시작점을 지정하는 과정

|
| :subtitle:`Step.30`

.. image:: /images/WorkingTest/step_30.jpg
   :width: 800

| :blackcircle:`●` 라인 상태를 확인하면서, 실시간으로 조그버튼을 돌려줍니다. 시계 방향으로 회전 시 노즐과 베드 간격이 커지며, 반시계는 좁아집니다.
| :blackcircle:`●` 간격이 클수록 라인이 얇게 나오며, 좁을수록 라인이 두껍게 나옵니다. 너무 얇아도 안되고, 너무 두꺼워도 출력에 문제가 됩니다.

|
| :subtitle:`Step.31`

.. image:: /images/Maintenance/38_Leveling_Line_1.png
   :width: 500
   :align: center

.. raw:: html

    <center-text-for-figure>꼭지점 부분이 휘어져 구불구불한 경우</center-text-for-figure>

|

.. image:: /images/Maintenance/39_Leveling_Line_2.jpg
   :width: 500
   :align: center

.. raw:: html

    <center-text-for-figure>규칙적으로 출력된 모습(정상)</center-text-for-figure>

|

.. image:: /images/Maintenance/43_Leveling_Line_3.jpg
   :width: 500
   :align: center

.. raw:: html

    <center-text-for-figure>레벨링이 많이 눌린 경우</center-text-for-figure>  

|

.. image:: /images/WorkingTest/step_31.jpg
   :width: 800

| :blackcircle:`●` 한번 더 레벨링을 실행하고 라인상태가 규칙적으로 출력되는지 확인합니다.
|

.. image:: /images/WorkingTest/CheckAfterLeveling.gif
   :width: 600
   :align: center

|
| :blackcircle:`●` 레벨링을 완료하고 손으로 긁었을 경우 쉽게 떨어지면 레벨링이 불안정한 상태입니다. 좀 더 낮춰주세요.
| :orangecircle:`●` 규칙적이라면, '저장'(1) 버튼을 눌러 레벨링을 완료합니다.

| ※ 레벨링 라인이 제대로 그려지지 않은 상태라면, 출력이 제대로 되지 않습니다. 레벨링 라인을 정확히 점검하시고 넘어가시기 바랍니다.
| ※ 레벨링 중 필라멘트가 뭉치거나 라인이 그려지지 않는다면, 베드와 노즐을 가까이 붙이는 방향으로 값을 조절해 보시기 바랍니다.
| ※ 구간별로 레벨링이 덜되거나 되지 않는 부분이 있다면, 메뉴 - 세부조정 - :ref:`Z보정 <targetZAdjust>` 을 진행해보시기 바랍니다.

|

필라멘트 삽입/제거
--------------------------

|
| :subtitle:`Step.32`

.. image:: /images/WorkingTest/step_32.jpg
   :width: 800

| :blackcircle:`●` 3D 프린팅 출력에 앞서 필라멘트가 연결되어 있어야 합니다.
| :blackcircle:`●` 필라멘트의 삽입, 제거, 무게설정 과정을 알아보도록 하겠습니다.
| :orangecircle:`●` 메인화면에서 '메뉴'(1)-'삽입/제거'(2) 버튼을 눌러줍니다.

|
| :subtitle:`Step.33`

.. image:: /images/WorkingTest/step_33.jpg
   :width: 800

| :blackcircle:`●` 이후 '삽입'(1) 버튼을 누릅니다. 예열되지 않은 상태라면, 예열을 하라는 팝업 창이 표시됩니다.
| :blackcircle:`●` 예열이 완료되면, 다시 시도합니다.
| ※ 필라멘트가 삽입되지 않는다면, :ref:`필라멘트가 삽입되지 않는 경우 <targetCannotInsertFila>` 항목을 참고하세요.

|
| :subtitle:`Step.34`

.. image:: /images/WorkingTest/step_34.jpg
   :width: 800

| :orangecircle:`●` 필라멘트를 손으로 잡고 있는 상태에서 '삽입'(1) 버튼을 눌러줍니다.
| :blackcircle:`●` 버튼을 누르게 되면, 삽입을 위한 동작을 시작합니다.
| :blackcircle:`●` 토출이 완료되면, 팝업창이 뜹니다.

|
| :subtitle:`Step.35`

.. image:: /images/WorkingTest/step_35.jpg
   :width: 800

| :orangecircle:`●` 반대로 필라멘트 제거 과정은 예열된 상태에서 '제거'(1) 버튼을 누르면, 필라멘트 제거 동작을 시작합니다.

|
| :subtitle:`Step.36`

.. image:: /images/WorkingTest/step_36.jpg
   :width: 800

| :blackcircle:`●` 필라멘트를 삽입 후엔 필라멘트의 무게를 설정해 주시는 것이 좋습니다.
| :orangecircle:`●` '무게 설정'(1) 버튼을 눌러줍니다.
| :blackcircle:`●` 현재 필라멘트량과 필라멘트의 밀도를 볼 수 있습니다.
| ※ 무게 설정을 하게 되면, 필라멘트의 현재 잔여 필라멘트를 파악할 수 있고, 출력할 모형을 출력할 재료가 충분한지 알 수 있습니다.

|
| :subtitle:`Step.37`

.. image:: /images/WorkingTest/step_37.jpg
   :width: 800

| :orangecircle:`●` 새로 삽입된 필라멘트 무게가 1kg라면 '1kg'(1) 버튼을 누릅니다.
| :blackcircle:`●` 1kg로 설정할 것인지 팝업창이 나타납니다. '예'를 누릅니다.

|
| :subtitle:`Step.38`

.. image:: /images/WorkingTest/step_38.jpg
   :width: 800

| :orangecircle:`●` 1kg, 3kg 이외의 무게를 입력하고 싶을 경우에는, 'Custom'(1) 버튼을 눌러 무게를 설정해 줍니다.
| :yellowcircle:`●` 필라멘트의 밀도를 변경하려면, '밀도'(2) 버튼을 눌러 변경해 줍니다.
| :blackcircle:`●` 필라멘트 무게, 밀도를 설정하는 과정은 필수는 아니며 선택사항입니다.

|

출력하기
--------------------------

|
| :subtitle:`Step.39`

.. image:: /images/WorkingTest/step_39.jpg
   :width: 800

| :orangecircle:`●` 메인화면에서 '출력'(1) 버튼을 눌러줍니다.
| :yellowcircle:`●` 출력 화면에서 'TFT SD'(2) 버튼을 눌러줍니다.

|
| :subtitle:`Step.40`

.. image:: /images/WorkingTest/step_40.jpg
   :width: 800

| :blackcircle:`●` 출력하고자 하는 파일을 선택해 줍니다.
| :blackcircle:`●` 재확인 차 팝업이 뜨면, 확인 버튼을 눌러 출력을 시작합니다.

|

완성된 출력물 제거하기
--------------------------

.. image:: /images/WorkingTest/Remove_Parts.png
   :width: 800

| :redbold:`※주의` : 완성된 출력물을 제거하기 위해서는 시트를 분리하여, 면적이 작은 출력물은 크게 상관 없지만, 면적이 큰 경우에는 천천히 살짝 구부린 다음 제거 해주시는 것이 좋습니다. 
| 면적이 큰 출력물은 제거하는 과정에서 시트를 급격히 구부린다거나 힘을 너무 준 상태로 출력물을 제거하려다 보면, :blackbold:`시트가 뜯길 수 있으니 주의해주시기 바랍니다.`
| :blackcircle:`●` 면적이 넓은 출력물은 베드를 약간 예열을 하고 제거하면 쉽게 제거 할 수 있습니다.

|

출력물 점검해보기
--------------------------

| 출력이 끝까지 된 경우에 점검해야 될 것과, 출력이 초반에 실패한 경우에 점검해야할 것들이 있습니다.

| :blackbold:`출력이 성공한 경우`
| 출력이 성공하였다면, 살펴봐야할 부분은 한가지입니다. 바닥면을 보고 레벨링이 잘 되었는지 확인하는 일입니다.

.. image:: /images/WorkingTest/1_TestParts_Bad.png
   :width: 800
   :align: center

.. raw:: html

   <center-text-for-figure>베드, 노즐 간격이 높은 경우 바닥면(왼), 옆면(오)</center-text-for-figure>

| 
| 먼저 출력이 되더라도 바닥면을 보았을 때 라인들의 틈이 보인다면, 레벨링이 좋지 않고 이후 출력에서 문제가 될 가능성이 높습니다. 이는 레벨링을 재설정하고 다시 출력해보시기 바랍니다.

.. image:: /images/WorkingTest/3_TestParts_Bad.png
   :width: 800
   :align: center

.. raw:: html

   <center-text-for-figure>베드, 노즐 간격이 낮은 경우 바닥면(왼), 옆면(오)</center-text-for-figure>

|
| 또한 출력물을 옆면에서 보았을 때, 바닥면 쪽이 삐죽 튀어나온 경우는 이후에도 출력은 가능하지만, 바닥면 부분이 퍼지는 증상이 있습니다. 이의 경우에도 레벨링을 재설정하면 증상이 완화됩니다.

.. image:: /images/WorkingTest/2_TestParts_Normal.png
   :width: 800
   :align: center

.. raw:: html

   <center-text-for-figure>베드, 노즐 간격이 적당한 경우 바닥면(왼), 옆면(오)</center-text-for-figure>


| 바닥면이 깔끔하다면, 이는 다음 출력도 정상적으로 출력될 가능성이 높습니다. 이제 :ref:`슬라이싱 프로그램 설치 <targerInstallCura>` 로 넘어가시면 됩니다.

| 
| :blackbold:`출력이 실패한 경우`
| 출력이 실패한 경우라면, 바닥면에서 실패할 경우가 높습니다. 대부분 레벨링과 관련된 문제입니다.

|
| 노즐 아래에서 필라멘트가 뭉치는 경우, 바닥면에 붙어 있다가 떨어지는 경우
| 이 경우는 레벨링이 제대로 되지 않았거나, 레벨링의 상태가 좋지 않습니다. 레벨링 과정에서 ㄹ 모양의 라인들이 그려졌는지 확인하고, :ref:`레벨링센서의 높이를 점검 <targetWorkingTest_SensorHeight>` 하시고, 이어서 :ref:`안착불량을 점검 <targetAbnormalPrinted_BadLanding>` 하세요.

|
| :blackbold:`위의 사진들을 보아도 판단이 되지 않는다면,` 네이버 공식 카페인 https://cafe.naver.com/cremaker 에 출력물 사진과 레벨링된 사진을 올려주시면 피드백드립니다.

|
| 이제 슬라이싱 프로그램을 설치하고 여러분들이 생각하는 것들을 출력해보세요.~
