## 새로 배운 내용
* Oracle이 기존의 MySQL이나 MariaDB와 다른점은 중간에 __리스너__ 가 있다는 점이다. 클라이언트가 데이터베이스 서버로 뭔가를 요청하기 위해서는 바로 서버로 요청을 하게 되는데,
Oracle의 경우에는 중간에 리스너라는게 있어서 리스너를 통해서 요청을 전달한다. _내 컴퓨터에서 리스너 포트는 1522번이다._
* 리스너가 로컬에서만 접근할 수 있도록 하는 설정이 있다. 만약 내 컴퓨터 이외의 컴퓨터에서 __원격으로 접속__ 하기 위해서는 아래의 명령어를 입력해서 해당 설정을 False로 설정해주어야 한다. 

        EXEC DBMS_XDB.SETLISTENERLOCALACCESS(FALSE);
  
* eclipse에서 RUN을 하기 위해선 __Crtl+F11__ 을 누르면 된다.

## 문제가 발생하거나 고민한 내용
* 이번에 유독 설치하는데 시간이 오래 걸리긴 했지만 다행히도 딱히 오류는 발생하지 않았다.

## 회고
* (+): 자바는 예전에 많이 다뤄본 언어라 자바 자체는 익숙하지만 그걸로 데이터베이스를 다뤄본 적은 처음이라 실습 과정에서 신기한 부분도 많고 새로운 내용도 많다. 또 다시 처음부터 배운다는 느낌으로 수업을 열심히 따라가야 할 것 같다.
* (-): 생각보다 설치하는데 시간이 오래 걸려서 제출 마감시간보다 몇시간이나 늦게 과제를 제출하게 됐다. 담부턴 좀 미리미리 하자.
* (!): 내 컴퓨터는 1521번 포트를 다른데서 이미 사용중이라고 떠서 리스너 포트를 1522번으로 설정했다. 이것때문에 간혹 교수님 코드를 그대로 따라했는데도 불구하고 오류가 발생하는 경우가 종종 있다. 그럴때는 당황하지 말고 침착하게 코드에서 1521 숫자를 찾아서 1522로 고치면 된다.