# 리눅스 HEAD 명령어


<div>
  <img width="400" src="https://github.com/myeonghuSong/linux_commandline/blob/master/img/head/zero.PNG?raw=true">
</div>

# 설명
- 문서 내용의 앞부분 출력
 
 
# 자주 사용되는 옵션
- -c, --bytes=[-]NUM
- -n, --lines=[-]NUM
    - byte 입력 시 K, M, G, T 입력 가능(예: 10M)
    - '-' 입력 시 문서의 마지막 NUM byte/line을 제외하고 출력(마지막 줄을 시작으로 밑에서 N줄 까지를 제외하고 모든 내용 출력) 


# 사용예제
- head /etc/passwd
- head -n 1 /etc/passwd
- cat /etc/passwd | head -n 15
- cat /etc/passwd | head -n -5

# screenshot


<div>
  <img width="400" src="https://github.com/myeonghuSong/linux_commandline/blob/master/img/head/first.PNG?raw=true">
</div>


<div>
  <img width="400" src="https://github.com/myeonghuSong/linux_commandline/blob/master/img/head/second.PNG?raw=true">
  <img width="400" src="https://github.com/myeonghuSong/linux_commandline/blob/master/img/head/third.PNG?raw=true">
</div>


- cat /etc/passwd | head -n 15
- 15줄이 출력되는 것을 볼 수 있다.


<div>
  <img width="400" src="https://github.com/myeonghuSong/linux_commandline/blob/master/img/head/fourth.PNG?raw=true">
  <img width="400" src="https://github.com/myeonghuSong/linux_commandline/blob/master/img/head/fifth.PNG?raw=true">
</div>
<div>
  <img width="400" src="https://github.com/myeonghuSong/linux_commandline/blob/master/img/head/sixth0.PNG?raw=true">
  <img width="400" src="https://github.com/myeonghuSong/linux_commandline/blob/master/img/head/sixth.PNG?raw=true">
</div>


- cat /etc/passwd | head -n -2 cat /etc/passwd | head -n -1 명령어를 수행한 결과
- -2 명령어를 수행하여 마지막 2줄을 제거한 후 출력하니 sshd로 시작하는 문자들이 보이는 것을 알 수 있다.
- -1 명령어를 수행하니 마지막 한 줄을 제외하고 모두 출력하여 sshd로 시작하는 문자들 다음 문자들이 나오는 것을 볼 수 있다.
