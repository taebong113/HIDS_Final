<h1>리눅스 우분에서의 네트워크 침입 탐지 시스템-IDS </h1>

1.네트워크 침입 탐지 룰을 생성(SNORT RULE)
2.20가지 이상 네트워크 공격 탐지 
3.탐지된 정보 DB에 로깅 
4.DB의 데이터를 웹 통해 모니터링 
5.네트워크 모의 해킹 실습 및 테스트


<h2>Attack Server</h2>
ip:192.168.64.3 OS(Kali Linux)
<h2>Tarbet Server</h2>
ip:192.168.64.15 ( Ubuntu)

<h2>Web server</h2>
웹 모니터링 (php, apache)

<h2>침입탐지도구</h2>
Snort
- 오픈소스 형태의 네트워크 인트라시온 탐지 시스템 <br>
Snort Rule
- Snort가 사용하는 규칙 세트 <br>
-Dos ATTACK 탐지 <br>
-SSH BRUTE FORCE ATTACK 탐지 <br>
-XMAS 포트 스캔 탐지 규칙 <br>
-LANDATTACK 탐지 규칙<br>

<h2>BARNYARD2 이용한 데이터 베이스 연동 </h2>
- BARNYARD2는 SNORT UNIFIED2 바이너리 출력 파일을 위한 오픈 소스 인터프리터.
- SNORT가 효율적인 방식으로 DB에 탐지된 로그를 로깅.

<h2>웹 화면 구성</h2>

기능적 구성 요소 <br>
1. 상단바 <br>
- 전체적인 탐지된 다양한 공격 유형 EVENT 발생수  (전체 이벤트 로그수, DOS,SNI,TEM,DET 총 5가지 공격유형)
2. 실시간 탐지된 공격 <br>
- 실시간으로 공격을 탐지하여 5개까지 출력.
3. 실시간 공격 경향 그래프<br>
- 실시간으로 탐지된 공격을 그래프로 시각화 
4. 최근 침입 로그<br>
- 탐지된 로그에 대한 정보를 출력 
5. 더보기 (침입 로그)<br>
- 지금까지 탐지된 모든 로그 출력


