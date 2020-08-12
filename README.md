1. 프로젝트를 구체화한다. (시나리오)
 - 시뮬레이터를 이용한 시연은 불가능 (물리적인 결과가 있어야한다.)
 ㄱ. 자율주행으로 차가 이동.
 ㄴ. 버튼을 눌르면 주차 모드로 변경.
 ㄷ. 주차 모드로 변경되면 가까운 경로에 있는(혹은 지정한 경로) 주차 경로를 따라서 주차를 한다.
 ㄹ. (필수는 아님) 주차 모드를 진행하던 도중 모드가 변경되면 다시 주행으로 변경.
 ㅁ. (필수는 아님) 영상 인식을 이용하여 운전자가 졸음 상태인지, 평상시 상태인지 구분하여 모드 변경.

2. 맵핑을 해서 위치를 인식하고 이 위치를 기반으로 주차 알고리즘을 구현한다.
 - 라이더, IMU, 카메라를 사용
 - 주차 공간을 여러개 만들어서 그 중 위치를 선택하면 그 위치로 경로 추종을 이용하여 주차하는 알고리즘 구현
 - 경로는 각 주차 공간마다 한 개씩 구현

3. 해야할 일
 ㄱ. 맵핑할 공간을 먼저 만들어야한다.
	- 맵이 만들어서 사용하면 위치가 이동하면 안된다. (위치가 변할 수 있음, 새로 맵핑을 해야한다.)
 ㄴ. 센서를 이용하여 맵핑을 하고 맵 안에서 위치를 정확하게 인식한다.
 ㄷ. 주차 공간을 선정하고 주차 공간으로 이동하는 경로를 만든다.