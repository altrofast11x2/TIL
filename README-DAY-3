1. netstat — 네트워크 상태 확인

네트워크 연결 상태와 포트 정보 등을 확인할 수 있습니다.

netstat -tuln


-t: TCP 연결

-u: UDP 연결

-l: 대기 중인 포트

-n: 숫자 형태로 주소와 포트 보기

2. ifconfig — 네트워크 인터페이스 정보

네트워크 인터페이스의 상태나 IP 주소를 확인할 때 사용합니다.

ifconfig


-a: 모든 네트워크 인터페이스 정보 보기

3. iwconfig — Wi-Fi 설정 확인

Wi-Fi 인터페이스의 상태를 확인하거나 설정할 수 있습니다.

iwconfig

4. nmap — 네트워크 스캐닝

특정 네트워크의 호스트나 포트를 스캔할 때 사용합니다. 이 명령어는 Kali에서 가장 많이 쓰이는 도구 중 하나입니다.

nmap -sP 192.168.1.0/24  # 네트워크에 연결된 모든 장치 찾기
nmap -sV 192.168.1.1  # 특정 IP에서 열린 포트와 서비스 버전 확인

5. whois — 도메인 정보 조회

도메인의 등록 정보(Whois 데이터)를 확인할 수 있습니다.

whois example.com

6. curl — URL 요청

웹사이트에 HTTP 요청을 보내고 응답을 받을 때 사용합니다.

curl -I http://example.com  # HTTP 헤더 정보만 보기
curl http://example.com  # 웹페이지 내용 출력

7. wget — 파일 다운로드

인터넷에서 파일을 다운로드할 때 사용합니다.

wget http://example.com/file.zip

8. tcpdump — 네트워크 패킷 캡처

네트워크를 통해 오가는 패킷을 캡처하고 분석할 때 사용합니다.

sudo tcpdump -i eth0


-i: 인터페이스 지정 (예: eth0, wlan0)

-w: 파일로 저장 (예: sudo tcpdump -i eth0 -w capture.pcap)

9. airmon-ng — Wi-Fi 모니터 모드 활성화

Wi-Fi 패킷 캡처 및 분석을 위해 무선 네트워크 카드에서 모니터 모드를 활성화할 때 사용합니다.

sudo airmon-ng start wlan0  # wlan0을 모니터 모드로 전환

10. aircrack-ng — Wi-Fi 비밀번호 크래킹

Wi-Fi 네트워크의 비밀번호를 크랙하는 도구입니다. (주의: 합법적인 환경에서만 사용해야 합니다.)

sudo aircrack-ng capture_file.cap  # 캡처된 패킷을 이용해 비밀번호 추출

11. chmod — 파일 권한 변경

파일이나 디렉터리의 접근 권한을 변경할 때 사용합니다.

chmod 777 file.txt  # 모든 사용자에게 읽기, 쓰기, 실행 권한 부여
chmod 644 file.txt  # 소유자는 읽기/쓰기, 다른 사용자는 읽기만 허용

12. chown — 파일 소유자 변경

파일이나 디렉터리의 소유자 및 그룹을 변경할 때 사용합니다.

sudo chown user:group file.txt

13. ps — 프로세스 상태 보기

현재 실행 중인 프로세스들을 확인할 수 있습니다.

ps aux  # 시스템의 모든 프로세스 보기

14. kill — 프로세스 종료

특정 프로세스를 종료할 때 사용합니다.

kill -9 PID  # 특정 프로세스를 종료


PID: 프로세스 ID

15. history — 명령어 히스토리 보기

자주 사용하는 명령어들을 확인할 수 있습니다.

history

16. find — 파일 찾기

시스템에서 특정 파일을 찾을 수 있습니다.

find / -name "file_name"  # 루트 디렉토리부터 "file_name"을 찾음
