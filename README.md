# :atm: 계좌 관리 서비스 AMS_1
<br />

## :page_facing_up: 목차
1. 프로젝트 소개
2. 프로젝트 기능
   * [계좌생성](#1.-계좌생성)
     * 입출금 통장
     * 마이너스 통장
   * 계좌목록 조회
   * 입금
   * 출금
   * 프로그램 종료
<br />

## :eyes: 1. 프로젝트 소개
메모리(배열)를 이용한 은행 계좌 목록 저장 및 관리 가능한 간단한 애플리케이션 (화면 : 콘솔창) 
<br /><br />

:calendar: 프로젝트 기간 : 2023년 5월 16일 <br />
:hammer: Tools : <img src="https://img.shields.io/badge/Eclipse-FE7A16.svg?style=for-the-badge&logo=Eclipse&logoColor=white" /> <br />
:books: languages : <img src="https://img.shields.io/badge/Java-007396?style=flat&logo=Openjdk&logoColor=white" /> <br />
<br />

## :pushpin: 2. 프로젝트 기능
### 0. 프로그램 시작
* boolean run = true 를 이용하여 while()문이 프로그램 종료하기 전까지 반복 실행하게 한다.
* 프로그램 시작 시 메뉴를 화면에 보여준 뒤에 사용자로 부터 메뉴 선택 값을 입력 받는다. <br />

![0 메뉴](https://github.com/HeeYeong91/project_ams1/assets/139057065/6ef8ae18-4bb5-4d12-a5f9-2a465bf63bf4)

### 1. 계좌생성
* 계좌 생성 시 입출금통장인지 마이너스통장인지 사용자로 부터 숫자를 입력 받아 선택하게 한다.
* 입출금통장 선택 시 예금주명, 비밀번호, 최초입금액을 사용자로부터 입력 받은 후 계좌를 등록한다.
* 마이너스통장 선택 시 예금주명, 비밀번호, 대출액을 사용자로부터 입력 받은 후 계좌를 등록한다. <br />

![1 계좌생성](https://github.com/HeeYeong91/project_ams1/assets/139057065/8b42bcec-d65f-4d0f-8ea9-9589ad2294b0)

### 2. 계좌목록 조회
* 계좌목록 조회 시 계좌번호 오름차순으로 입출금통장, 마이너스 통장 모두 화면에 출력한다.
* 계좌종류 / 계좌번호 / 예금주명 / 비밀번호 / 잔액 / 대출금 으로 구분해서 화면에 출력한다.
* 비밀번호는 '*'로 보여준다.
* 마이너스 통장은 대출금 표시 후 잔액에는 마이너스 금액을 보여준다. <br />

![2 계좌목록](https://github.com/HeeYeong91/project_ams1/assets/139057065/989311d3-47e1-49f3-9d55-cd318a37c931)

### 3. 입금
* 입금 시 입금 할 계좌번호를 사용자로부터 입력 받는다.
* 계좌번호가 존재하면 입금액을 입력 받는다.
* 입금계좌가 마이너스통장일 경우 대출금에서 빼주고 화면에 입금액과 대출잔액을 보여준다.
* 입금계좌가 입출금통장일 경우 화면에 입금액과 입금 후 잔액을 보여준다.
* 계좌번호가 존재하지 않을 때는 "입력하신 계좌가 존재하지 않습니다" 메세지를 화면에 보여준다. <br />

![3 입금](https://github.com/HeeYeong91/project_ams1/assets/139057065/96c9970d-314d-4823-afc1-93dbb7327337)

### 4. 출금
* 계좌번호를 사용자로부터 입력 받는다.
* 비밀번호를 입력받고 비밀번호가 맞다면 출금액을 입력 받는다.
* 비밀번호가 다르면 "비밀번호를 확인하세요" 메세지를 화면에 보여준다.
* 계좌 종류가 마이너스통장일 경우 대출금을 출금 금액만큼 올리고 화면에 해당금액이 대출되었다는 메세지와 총 대출액을 보여준다.
* 입출금통장일 경우 해당 금액이 출금되었습니다. 메세지와 잔액을 보여준다.
* 입출금통장일 경우 잔액이 부족할 경우 "계좌 잔액이 부족합니다." 메세지를 화면에 보여준다. <br />

![4 출금](https://github.com/HeeYeong91/project_ams1/assets/139057065/90847e9b-3665-4edf-9699-889471e2789c)

### 5. 프로그램 종료
* 프로그램을 종료할 시 while()문으로 동작하고 있는 프로그램을 종료하기 위해
* boolean run 값을 false로 변경한다. <br />

![5 종료](https://github.com/HeeYeong91/project_ams1/assets/139057065/50f82ba1-9b84-4e24-8618-c66ac32e59c2)
