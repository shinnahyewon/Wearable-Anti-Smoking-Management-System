# Wearable-Anti-Smoking-Management-System
Wearable Anti-Smoking Management System

■ 프로젝트 개요
1) 개발 배경
 금연은 남녀노소 나이 불문 모두에게 중요하고 담배가 건강에 해가 되는 만큼 금연의 중요성이
강조되고 있다. 담배가 중독성이 강한 만큼 금연하기에 어려움이 있어 금연에 도움이 되고자 프로젝트를 기획하게 되었다.

2) 개발 목표
사용자의 워치에 사용을 목표로 웨어러블 디바이스로 개발하였고, 일정 수준의 가스가 센서에 감지되면 워치에 진동을 통해 경고를 주며 감지 횟수를 카운터 한다. 하루 동안의 사용자의 담배 감지 횟수를 DB에 저장하여 관제센터에 전송하여 하루가 끝났을 때 사용자에게 오늘의 금연 횟수와 금연의 성공 여부를 알려주며 오작동의 우려가 있어 진동 강제 종료 기능을 추가하여 사용자의 금연에 도움을 줄 수 있음을 기대한다.
■ 시스템 구성!
[image](https://github.com/shinnahyewon/Wearable-Anti-Smoking-Management-System/assets/161293023/7c1bd7c1-68a7-4db7-9d42-ef914b15a90b)

![image](https://github.com/shinnahyewon/Wearable-Anti-Smoking-Management-System/assets/161293023/71bad07d-77bd-4414-a66b-abf398da714a)

■ 주 시스템
1) 가스 감지
 가스 센서에 일정 값 이상 감지되면 OLED에 Cigarette detection!! 출력과 동시에 DC 모터 작동(진동을 대신하여 사용), 평소 시계로도 사용 가능하게 시계 기능 구현.
![image](https://github.com/shinnahyewon/Wearable-Anti-Smoking-Management-System/assets/161293023/29a00e6c-59f1-4a34-9357-039d0653c028)
2) 오작동 강제 종료 버튼
 오작동과 간접흡연 등 다양한 환경에서 흡연을 하지 않음에도 센서가 작동될 경우를 대비해
핸드폰으로 모터 제어 버튼을 눌러 오작동 시 강제 종료되게 구현.
![image](https://github.com/shinnahyewon/Wearable-Anti-Smoking-Management-System/assets/161293023/3bd19d0b-4903-456b-9447-bcf50ab009c3)
3) 디바이스로부터 받은 데이터 관리
 그룹별로 USER1, USER2... 테이블에 하루 동안의 흡연 횟수를 날짜별로 저장함.
![image](https://github.com/shinnahyewon/Wearable-Anti-Smoking-Management-System/assets/161293023/cd29bbea-e4b0-4606-b402-f836b875f6a2)
![image](https://github.com/shinnahyewon/Wearable-Anti-Smoking-Management-System/assets/161293023/af633a19-5f80-42d3-bb5d-7eb4bcd92605)
![image](https://github.com/shinnahyewon/Wearable-Anti-Smoking-Management-System/assets/161293023/9bdc1bf5-11b6-4a60-94a6-ce0a21580e1a)
4) 성공 여부를 LCD에 출력
 서버에서 하루 동안의 흡연 횟수를 받아 그룹 구성원의 하루 흡연 성공 여부를 LCD에 출력한다.
![image](https://github.com/shinnahyewon/Wearable-Anti-Smoking-Management-System/assets/161293023/edaa788c-1e42-4ef2-b046-2e96e40eb198)
■ 기대 효과
- 기존의 금연 팔찌의 문제점을 개선.
- 흡연자에게 경각심을 줌.
- 하루 동안의 자신의 흡연 횟수를 확인함으로 흡연 횟수 감소 기대.
