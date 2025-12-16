  **Termux & GitHub 오늘 배운 내용 정리** 

오늘 학습에서는 Android 환경에서 Termux를 활용해 기본적인 리눅스 명령어를 사용하고, 간단한 웹 서버를 실행하며, Git과 GitHub을 이용한 프로젝트 관리 방법을 배웠습니다.

1. **경로 및 디렉터리 명령어**

   * `pwd`로 현재 위치를 확인할 수 있음을 배웠습니다.
   * `cd ~`로 홈 디렉터리로 이동하고, `mkdir Web`으로 새 디렉터리를 생성한 뒤 `cd Web`으로 이동하는 방법을 실습했습니다.
   * `ls`와 `ls -la`를 통해 파일과 숨김 파일 목록을 확인할 수 있음을 확인했습니다.

2. **파일 관리**

   * `touch 파일명`으로 새 파일을 만들 수 있다는 것을 배웠습니다.
   * `cat 파일명`과 `less index.html`로 파일 내용을 확인할 수 있음을 실습했습니다.
   * 필요 없는 폴더를 삭제할 때는 `rm -rf 폴더명`을 사용할 수 있다는 것도 배웠습니다.
   * 설치한 패키지를 삭제할 때는 `pkg uninstall 패키지명` 명령어를 사용할 수 있음을 배웠습니다.

3. **파일 편집 (nano)**

   * `nano 파일명`으로 파일을 편집할 수 있으며, `CTRL + O`로 저장하고 `CTRL + X`로 종료하는 방법을 실습했습니다.

4. **웹 서버 실행 (Python)**

   * `python -m http.server 8000`으로 간단한 웹 서버를 실행할 수 있음을 배웠습니다.
   * 로컬 주소 `http://127.0.0.1:8000/`에서 확인 가능하며, 서버 종료는 `CTRL + C`를 사용합니다.

5. **패키지 관리**

   * `pkg update && pkg upgrade`으로 Termux 패키지를 최신 상태로 유지할 수 있음을 배웠습니다.
   * `pkg install git`으로 Git을 설치하고, `git --version`으로 설치 여부를 확인했습니다.
   * `pkg uninstall 패키지명`으로 설치된 패키지를 삭제할 수 있습니다.

6. **Git 기본 개념 및 사용법**

   * Git은 로컬에서 파일 변경 이력을 관리하는 도구입니다.
   * `git init`으로 저장소를 초기화하고, `git add .`로 변경 사항을 스테이징하며,
     `git commit -m "메시지"`로 작업 상태를 저장할 수 있음을 배웠습니다.
   * `git config --global user.name "이름"`과 `git config --global user.email "이메일"`로 커밋 작성자 정보를 설정할 수 있으며, 이는 GitHub 로그인과는 별개입니다.

7. **GitHub 연동**

   * `gh auth login`을 통해 GitHub 계정과 Termux를 연동하고, 브라우저에서 인증하는 방법을 실습했습니다.
   * `gh auth status`로 로그인 상태를 확인할 수 있으며, 원격 저장소는 `git remote -v`로 확인할 수 있습니다.

**정리하면**, 오늘은 Termux에서 기본 명령어 사용, 파일 생성/편집, Python 웹 서버 실행, Git과 GitHub 연동까지 프로젝트 관리의 기초 과정을 배웠습니다.
이 과정을 통해 Android 환경에서도 로컬 개발과 버전 관리, 원격 업로드까지 연결할 수 있는 능력을 익혔습니다.

---

---------**오늘 배운 명령어 정리**---------------------------------------------------------------------------------------------------------------

```
pkg update         # 패키지 목록 새로고침
pkg upgrade        # 설치된 패키지 업그레이드
pkg install 이름   # 패키지 설치
pkg uninstall 이름 # 패키지 설치삭제
pkg search 이름
pwd               # 현재 위치 확인
cd ~             # 홈 디렉터리 이동
cd 폴더명   # 폴더 이동
cd ..      # 폴더 뒤로 이동
cp a.txt b.txt      # 파일 복사
mv a.txt b.txt      # 이름 변경
mv a.txt folder/    # 파일 이동
cp -r 폴더1 폴더2   # 폴더 복사
ls               # 파일 목록 확인
ls -la           # 숨김파일 + 상세 정보
mkdir 폴더명        # 새 디렉터리 생성
touch index.html    # 파일 생성
cat 파일명   # 파일 내용 출력
less 파일명  # 스크롤 가능한 읽기
rm 파일명    # 파일삭제
rm -rf 폴더명    # 폴더 강제 삭제
rm 파일명        #파일 삭제
rmdir 폴더명        # 폴더가 비어 있을 때만 삭제 가능
rm -r 폴더명        # 안에 파일 있어도 삭제 (가장 많이 사용함)
rm -ri 폴더명       # 하나씩 물어보며 안전 삭제
rm -rf 폴더명       # 경고 없이 전부 삭제 
pkg update && pkg upgrade  # 패키지 최신화
pkg install git           # Git 설치
pkg uninstall 패키지명    # 패키지 삭제
git --version             # Git 설치 확인
git init                  # Git 저장소 초기화
git add .                 # 모든 변경 파일 스테이징
git commit -m "메시지"     # 커밋 생성
git config --global user.name "이름"   # 사용자 이름 설정
git config --global user.email "이메일" # 이메일 설정
gh auth login             # GitHub CLI 로그인
gh auth status            # GitHub 로그인 상태 확인
git remote -v             # 원격 저장소 확인
python -m http.server 8000 # 웹 서버 실행
CTRL + C                  # 웹 서버 종료
nano index.html           # 파일 편집
CTRL + O                  # nano 저장
CTRL + X                  # nano 종료

Made By git hub: Altrofast11x2 (BY-NC-ND)
