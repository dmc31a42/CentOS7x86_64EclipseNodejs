# CentOS7x86_64EclipseNodejs
Step Install and Configure Node.js Integrated Development Environment in CentOS7(x86_64)

# Installation
## CentOS 7 Install
* Language : Korean
* Software select(소프트웨어 선택) : WorkStation for Development and Creation(개발 및 창조를 위한 워크스테이션), Other option disable
* Install Target(설치 대상) : Auto(Click->Finish완료)
* **Network & Host Name** : 
  * Ethernet(이더넷) Off->On
  * Option(설정)->General(일반)->When available, Connect this network automatically(사용 가능하면 자동으로 이 네트워크에 연결)
  * Host Name : as you wish.
* Root password, User create

## CentOS 7 Configure
* VMware tools : http://partnerweb.vmware.com/GOSIG/CentOS_7.html
관리자 계정에서 작업을 한다.
```
yum install open-vm-tools
```
나오는 질문에 y를 입력하여 설치를 완료하면 자동으로 실행된다.

* Java install
```
yum install java-1.8.0-openjdk java-1.8.0-openjdk-devel
```
또는 여기서 참고 http://pentode.tistory.com/45

* Eclipse install
  * http://www.eclipse.org/downloads/ 에서 eclipse-inst-linux64.tar.gz 다운 
  ```bash
  [root@localhost download]# tar -xvzf eclipse-inst-linux64.tar.gz
  ```
  ```bash
  [root@ localhost eclipse-installer]# ./eclipse-inst
  ```
  * 필요한거 고른 후 설치 경로만 /root/~ 에서 /opt/~ 로 바꿔주면 됨
  
