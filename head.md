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
