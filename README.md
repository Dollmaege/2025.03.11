# 2025.03.11

restful하게 만든다.

http request method
서버 구조에서 요청(request)과 응답(response)가 이루어지는 방식을 의미한다.

GET : 조회 메서드
- 특정 조건을 전달하고 싶으면 쿼리스트링으로 전달

POST : 전달한 데이터를 처리/추가하는 메서드
- 주로 신규 리소스 등록, 프로세스 처리에 사용

PUT : 리소스를 대체(수정)하는 메서드
- 요청 메시지에 리소스가 있으면 덮어쓰고, 없으면 새로 생성한다.

PATCH : 리소스의 일부분을 변경하는 메서드

DELETE : 리소스 제거하는 메서드

1. 자료형
2. 변수
3. 연산자
4. 제어문
ㄴif, switch
ㄴfor, while, break, continue
5. 배열
6. 객체
7. 함수, 메서드
8. 이벤트, 이벤트 처리

노드js가 발달이되면서 웹콘솔에서 확인해야하는 js를 터미널(cmd)에서 확인이 가능하다.

C : CREATE 회원가입, 게시글작성
R : READ 로그인, 게시글보기
U : UPDATE 수정
D : DELETE 게시글삭제, 회원탈퇴 

this : 자기 자신에 대한참조
메서드 안에서의 this -> 메서드를 소유한 객체를 참조

객체안에서는 일반적인 모양의 함수는 ok 
하지만 화살표 함수는 this 를 인식을못함
화살표함수 내부에서 사용하는 this 는 함수를 포함하고 있는 객체를 참조하지 못한다. 

DOMcontentLoaded
동기방식 -> 하나의 명령이 끝나는대로 다음명령을 수행
HTML요소가 아직 만들어지지 않은 상태에서 기능을 추가하라고 하니까 에러가 발생
순차적으로 실행이 되니까 꼬이는 문제가 발생

비동기방식 -> 당장 처리해야할 명령과 나중에 처리해야할 명령을 구분할 수 있다.

배포(deploy)
웹페이지를 인터넷이랑 연결하여 누구나 접속해 볼 수 있는 상태로 만드는 행위
html, css, js -> 우리컴퓨터에서만 볼 수 있음(로컬환경)

웹페이지 배포 절차 
1. 웹 페이지를 컵퓨터에 저장한다.
2. 컴퓨터를 인터넷에 연결한다.
3. 컴퓨터의 설정을 변경하여 외부에서 접속할 수 있도록 한다.
4. 외부에서 접속을 요청 할 떄마다, 컴퓨터가 웹페이지를 보여줌

이때 사용된 컴퓨터를 서버(server)라고 부른다.

웹 호스팅 서비스

서버 용도로 사용되는 컴퓨터는 일반 컴퓨터보다 바싸다.
인터넷 회선도 무료가 아님.

서버를 많이 구매한 다음, 인터넷 회선에 가입하고, 서버를 빌려주는 회사들이 존재한다. 이러한 서비스를 웹 호스팅 이라고 부른다.
서버컴퓨터는 사양이 아주 높기 떄문에 하나의 서버에서 홈페이지를 수십, 수백개까지 운영할 수 있다.

cafe24, 가비아 등
aws, 

github 페이지
깃허브에서는 모료로 웹페이지를 호스팅 할 수 있는 서비스를 제공한다.

레포지토리로 이동 -> settings-> 왼쪽메뉴에 pages
->vranch에 master or main 설정
주의해야 할 점
root 폴더에 index.html이 존재해야 한다. 

지킬
프레임워크
지킬생태계(ECO-SYSTEM)
생태계라고 부를만큼 다양한 사용자들이 존재한다.
지킬로 만든 자기 작품을 많이 공유한다.

MIT 라이센드
이 소프트웨어를 누구든지 무상으로 제한없이 사요ㅕㅇ해도 좋다.
간, 완성된 소프트웨어의 중요한 부분에 저작권 표시를 해야한다.
소프트웨어의 원작자는 아무런 책임을 지지 않는다.

레포지토리의 포크
레포지토리의 복제본을 만드는 방식중 하나이다.
원본 레포지토리의 내용이 수정되거나, 삭제 되더라도 현재의 버전을 간직해두고 사용할 수 있다.
현재 버전의 레포지토리를 박제하는 행위

템플릿의 이해
우리가 가져온 템플릿의 html , css, js 를 건드릴 필요없이
내용정도만 수정을 하면 된다.

git init -> 해당폴더를 git 이 관리하겠다.
git remote -> 원격repo와 연결하겠다.
git add -> 해당폴더에 있는파일을 stage 에 올리겠다
git commit -m init -> git이 관리하도록 commit을 하겠다.
git origin master -> commit된 정보를 원격repo에 올리겠다.

gem uninstall jekyll -> 지킬 삭제
gem install jekyll -v '4.3.3' -> 특정 버전을 다운받을수있다.

yml 은 환경설정에 관련된 파일이다.
yml 파일의 주석은 # 이다.

_data -> 웹사이트 에서 활용할 데이터를 저장할 수 있다.
_includes -> 웹 페이지에 포함시킬 html 파일 저장
_layouts -> 웹 페이지의 뼈대를 결정 html 파일들이 들어감
_hosts -> 블로그 게시물을 저장
_sass -> css의기능을 확장시켜 더효율적이고 유지보수하기 쉬운 스타일 시트를 작성할 수있도록 도와준다.
_site -> 빌드가 끝난 코드가 저장된다.
코드를 다 작성하고 마지막에는 빌드라는 작업을 통해 데이터가 조립되어 배포에 적합한 상태로 다듬어진다.
실제로 배포할때는 빌드된 코드만 사용된다.

