# rust-reversing-helper

A ida script to help reversing rust binary

![](https://raw.githubusercontent.com/cha5126568/rust-reversing-helper/master/pic/diff_dis.png)
![](https://raw.githubusercontent.com/cha5126568/rust-reversing-helper/master/pic/d2.png)
![](https://raw.githubusercontent.com/cha5126568/rust-reversing-helper/master/pic/graph.PNG)

## 사용법

1. https://github.com/luser/rustfilt
이거 설치해서 스크립트에 있는 rustfilt 경로 바꿔주세요.
2. IDA 7.0 에서 스크립트 불러와주면 끝!

## 주의사항
1. 기본적 ELF x64만 지원합니다. 
exe는 인자를 바로 잡는 기능에서 문제가 생길겁니다.(fastcall 에서 리눅스랑 윈도우랑 인자 넣는 순서가 달라요..ㅜㅜ)

## 기능
1. 함수이름을 전부 디맹글링 해줍니다. (function name demangle)
2. 사용되는 문자열을 잡아줍니다. (string recovery)
3. 제대로 잡히지 않는 인자를 바로 잡아 줍니다. (argument recovery)
## TODO
- [ ] 다양한 바이너리로 테스트
- [ ] exe 지원
