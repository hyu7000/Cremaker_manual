레벨링이 지속적으로 바뀌는 경우
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
| 레벨링이 지속적으로 바뀌는 경우는 드물긴 하지만 있긴 합니다. 여기서 지속적이라하면, 레벨링을 설정하고 아무 변경사항 없이 다시 레벨링을 해도 높이가 달라지는 상황을 의미합니다. 이런 경우는 센서부분과 Z 구동부분을 살펴봐야 합니다.

|
| :blackbold:`1. 센서 높이가 노즐보다 많이 높은 경우`

|
| 센서가 제대로 고정되어 있는지 확인합니다. 또한 센서의 높이가 노즐보다 높게 있어야 하는게 맞지만 정상 범위보다 더 많이 높게 있는지 확인해봐야 합니다. (참조 :ref:`센서 높이 <targetWorkingTest_SensorHeight>` )

|
| :blackbold:`2. 리드스크류가 약간 헐겁게 체결된 경우`

|
| 리드스크류가 헐겁게 체결된 경우에도 레벨링이 지속적으로 변경될 수 있습니다.
| 리드스크류를 고정하는 커플러의 볼트 2개를 살짝 풀었다가 다시 조여보시기 바랍니다. (참조 :ref:`리드스크류 조립 <targetAssem3_Step28_AssemLeadScrew>` )

|
| :blackbold:`3. 온도 보정값의 이상`

|
| 간혹 레벨링 센서의 온도보정값이 불량하면, 레벨링이 종종 뒤틀릴 때가 있습니다.
| 이런 경우에는 메뉴-설정-기계-명령어에서 :blackbold:`M871 R` 을 입력하고 보내기 버튼을 누릅니다.
| 온도 보정을 초기화하는 명령어입니다.