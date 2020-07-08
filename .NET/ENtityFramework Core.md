<p>2020.07.08</p>

<h2> ASP.NET MVC </h2>
<label> EntityFramework Core </label>

<pre>
  EntityFramework 1.0 ~ 6.0 == .net Framework
  
  ASP.NET Core (7.0) == EntityFramework Core
  
  EntityFramework + Linq
    ==> user.where(u=>u.userNo = 1 이런 식으로 DB 검색 가능
</pre>

<h3>EntityFramework 개발 방식 2가지</h3>
<pre>
  1. Database First 방식 : Database DBA(데이터베이스 관리자)가 설계 + 물리적 데이터베이스 완성 상태
                          Database 기준으로 Application 개발
                          대규모 프로젝트에서 진행
  2. Code First 방식 : Code에서 Database 생성해 Application 개발
</pre>


<h3>SQL</h3>
<pre>
  SQL : <b>S</b>tructured <b>Q</b>uery <b>L</b>anguage
        관계형 데이터베이스 관리 시스템
  
  대표적인 SQL 3가지
  1. MS SQL Server(유료)
      : Developer DB(무료)
        Express (무료 - 소규모 개발, 공부)
  2. Oracle
  3. MySql
  
  Mobile) SQLite - 안드로이드 ,iOS
          NoSql
</pre>

<h3><s>Mac에 Local mySql 설치하기</s></h3>
<pre><s>
  1. <a href="https://dev.mysql.com/downloads/mysql/">MacOS MySQL</a> 에서 DMG file 다운로드
  2. id : root 로 자동 설정됨
     pw : 12345678 로 설정하기
  3. 환경설정에서 확인 가능
</s></pre>

<h3>Mac에 SQL Server 환경 만들기</h3>
<h4>SQL 엔진</h4>
<pre>
  참고 : <a href="https://docs.microsoft.com/ko-kr/sql/linux/quickstart-install-connect-docker?view=sql-server-linux-2017&pivots=cs1-bash#pullandrun2017">SQL Server 2017 docker Linux 설치 문서</a>
  1. Mac console에서 <b>sudo docker pull mcr.microsoft.com/mssql/server:2017-latest</b> 실행
  2. sudo docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=<내 비밀번호 설정(8자 이상)>" \
     -p 1433:1433 --name sql1 \
     -d \ mcr.microsoft.com/mssql/server:2017-latest
  2-1. 비밀번호 설정은 Password 로 했음
  3. sudo docker exec -it sql1 "bash" 로 SQL Server에 연결
</pre>
<h4>Workbench</h4>
<pre>
  DBeaver 사용했음ㅎㅎ
</pre>
