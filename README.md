# Back-end-Develop-Practice

## 1st Assignment

<h3> Eclipse, Spring 설치 </h3>

<details><summary style="color:skyblue"> JDK 1.8 설치 완료 </summary>

![JDK 1.8](./img/jdk1.8-setting.png)

</details>

<br>

<details><summary style="color:skyblue"> Eclipse 설치 완료 </summary>

![Eclipse](./img/eclipse-setting.png)

</details>

<br>

<details><summary style="color:skyblue"> Spring 설치 완료 </summary>

![Spring](./img/spring-setting.png)

</details>

<br>

<details><summary style="color:skyblue"> Tomcat 설치 완료 </summary>

![Tomcat](./img/tomcat-setting.png)

</details>

<br>

<details><summary style="color:skyblue"> mariadb, mysql Workbench 설치 및 샘플 DB 구축 </summary>

![MariaDB](./img/mariadb-setting.png)

</details>

<br>

<details><summary style="color:skyblue"> 스프링, Mariadb, MyBatis 연동, 데이터 조회 </summary>

![Server](./img/server-setting.png)

<details> <summary style="color:white"> POM.xml 수정 완료 </summary>

- springframework, java version 수정

![Version1](./img/pom-setting_1.png)


- mariaDB, mybatis dependency 추가

![Version2](./img/pom-setting_2.png)

- maven-compiler-plugin version 수정

![Version3](./img/pom-setting_3.png)


</details>
<br>
<details> <summary style="color:white"> root-context.xml 수정 완료 </summary>

- xsi:schemaLocation 추가, dataSource 수정

![RootContext](./img/rootcontext-setting.png)

</details>
<br>
<details> <summary style="color:white"> mybatis-config.xml, logback.xml, log4jdbc.log4j2.properties, test.xml 작성 완료 </summary>

- Resource Tree 

![ResourceTree](./img/resourcetree-setting.png)

- mybatis-config.xml 

![Mybatis](./img/mybatis-setting.png)

- logback.xml 

![Logback](./img/logback-setting.png)

- log4jdbc.log4j2.properties 

![Properties](./img/properties-setting.png)

- test.xml 

![Test](./img/test-setting.png)

</details>
<br>
<details> <summary style="color:white"> MovieDAO, MovieService, MovieVO, HomeController 작성 완료 </summary>

- Java Tree

![JavaTree](./img/javatree-setting.png)

- MovieDAO, MovieDAOlmpl 

![DAO1](./img/dao_1.png)
![DAO2](./img/dao_2.png)

- MovieService, MovieServicelmpl 

![Service1](./img/service_1.png)
![Service2](./img/service_2.png)

- HomeController

![Home](./img/homecontroller.png)

- MovieVO

![VO](./img/vo.png)

</details>
<br>
<details> <summary style="color:white"> Tomcat Address 수정 완료 </summary>

- /settingweb -> / 수정

![Address](./img/address-settig.png)

</details>

</details>

<br>

## 2st Assignment

<details> <summary style="color:skyblue"> API 문서 초안 작성 </summary>

https://brian-jung.gitbook.io/api-docs/eveinformation/eveintroduction

</details>

<br>

## 3st Assignment

<h3> RestController를 활용한 간단 API 구현 </h3>

- RestController를 사용한 간단한 API (20년도 로그인 수)를 구현합니다.
- 본 과정은 Spring Boot를 활용합니다.

<br>

<h3> 스프링부트 개발 환경 설정하기 </h3>

<details> <summary style="color:skyblue"> 프로젝트 세팅 완료 </summary>
<br>

- File > New > Project > Spring Boot > Spring Starter Project를 클릭하여 프로젝트 생성합니다.

![SpringBoot0](./img/springboot-start_1.png)

- API를 만들기 위함이니 Spring Boot Devtools, Spring Web, MyBatis Framework 만 선택합니다.

![SpringBoot1](./img/springboot-start_2.png)

![SpringBoot2](./img/springboot-start.png)

</details>

<br>

<details> <summary style="color:skyblue"> Pom.xml 수정 완료 </summary>

- Dependency를 수정합니다. Dependency에는 DB 관련 내용을 포함합니다.

![BootPOM0](./img/boot-pom_1.png)

![BootPOM1](./img/boot-pom_2.png)

![BootPOM2](./img/boot-pom_3.png)

</details>

<br>

<details> <summary style="color:skyblue"> application.properties 수정 완료 </summary>

- port, contextpath, view, db 등 각종 설정을 한 곳에서 진행합니다.
- 설정 내용은 serverport, contextpath를 진행하였습니다.
- suffix에 jsp를 줌으로써 /WEB-INF/views 아래에 jsp 파일을 자동으로 Mapping해주도록 합니다.

![AppPP0](./img/app-properties_1.png)

![AppPP1](./img/app-properties_2.png)

</details>

<br>

<details> <summary style="color:skyblue"> 기본 TEST </summary>

- test로 호출을 하면 test.jsp로 값을 전달한 화면이 보여짐을 확인할 수 있습니다. 
- 아래와 같이 [src > main] 아래에 webapp, views 폴더를 차례로 만들고 test.jsp를 만듭니다.

![TEST0](./img/boot-test_1.png)

![TEST1](./img/boot-test_2.png)

- com.devfun.settingweb_boot.test 패키지를 만들고 settingTest.java를 만들어 아래와 같은 컨트롤러를 작성합니다.

![TEST2](./img/boot-test_3.png)

- 프로젝트를 실행 후 /test를 호출해봅니다.
- 이때 실행은 SettingwebBootApplication.java에서 실행합니다.
- port는 application.properties에 등록되어 있습니다.
- 최종 URL : http://localhost:8031/test

![TEST3](./img/boot-test_4.png)

</details>

<br>

<details> <summary style="color:skyblue"> 통계(SW활용현황) API를 위한 DB, TABLE 생성 </summary>

- mysql Workbench를 이용하여 DB, TABLE을 생성합니다.
- 데이터는 임의로 넣어 사용합니다.

![BOOTDB0](./img/boot-db_1.png)
![BOOTDB3](./img/boot-db_3.png)
![BOOTDB1](./img/boot-db_2.png)

</details>

<br>

<details> <summary style="color:skyblue"> Spring Boot, Mybatis, mariadb 연동 </summary>

- 최종 URL : http://localhost:8031/sqlyearStatistic?year=20
- 조회하는 URL 임으로 GET으로 조회를 하여 url에 parameter를 입력합니다.
- 그 결과로 아래와 같이 JSON 구조 값이 나옴을 확인할 수 있습니다.

![BOOT0](./img/boot_0.png)

- 아래의 이미지대로 package, mapper, config, settingTest를 작성하여 API를 만듭니다.

![BOOT1](./img/boot_1.png)


<details> <summary style="color:white"> mybatis 설정 </summary>

- JAVA로도 config 설정이 가능합니다.
- DB와 mybatis를 활용하기 위한 설정 코드를 작성합니다.
- MapperScan 어노테이션을 활용하여 스캔할 패키지를 입력합니다.

![BOOT2](./img/boot-mybatis.png)
</details>

<br>

<details> <summary style="color:white"> mapper 작성 </summary>

- StatisticMapper interface 작성

![BOOT3](./img/boot-mapper.png)

- StatisticMapper 안에 쿼리를 정의합니다.
- 대표  restController로 [해당년도의 로그인 수]를 알기 위한 쿼리를 작성합니다.

![BOOT4](./img/boot-mapper_2.png)

</details>

<br>

<details> <summary style="color:white"> Service (비즈니스 Logic) 작성 </summary>

- interface로 yearloginNum을 정의합니다.

![BOOT5](./img/boot-service_0.png)

- JSON 값을 만들기 위해 HashMap 형태로 Return을 합니다.
- HashMap 값을 year, is_success, 쿼리로 가져온 cnt값으로 JSON 값을 만듭니다.

![BOOT6](./img/boot-service_1.png)

</details>

<br>

<details> <summary style="color:white"> settingTest 코드 추가  </summary>

![BOOT7](./img/boot-settingtest.png)

</details>

</details>

<br>

## 4st Assignment

<details> <summary style="color:skyblue"> 통계 API 구축 SQL문 </summary>

- 연간 접속자 수
    
    select count(*) as totCnt

	from statistic.requestinfo ri

	where left(ri.createDate, 2) = #{year};

- 월간 접속자 수
    
    select count(*) as totCnt

	from statistic.requestinfo ri

	where left(ri.createDate, 4) = #{month};
- 일간 접속자 수

    select count(*) as totCnt

	from statistic.requestinfo ri

	where left(ri.createDate, 6) = #{day};
- 평균 하루 로그인 수

    select count(*) / DAY(LAST_DAY(STR_TO_DATE(createDate, '%y%m%d%h%i'))) as avgCnt

	from statistic.requestinfo ri

	where left(ri.createDate,4) = #{avgday};
- 휴일을 제외한 로그인 수
- 부서별 월별 로그인 수

</details>

<br>

<details> <summary style="color:skyblue"> 통계 API 파일 작성 </summary>

- DAO
    - <statisticMapper.java>
    
    <br>
    
    ![statisticMapper0](./img/statisticMapper_0.png)
    
    - <statisticMapper.xml>
    
    ![statisticMapper1](./img/statisticMapper.png)

- SERVICE
    - <statisticService.java>
    
    <br>
    
    ![statisticService0](./img/statisticService_0.png)
    
    - <statisticService.xml>
    
    <br>
    
    ![statisticService1](./img/statisticService_1.png)

- TEST
    - <settingTest.java>
    
    <br>
    
    ![settingTest0](./img/settingTest.png)

</details>

<br>

<details> <summary style="color:skyblue"> 통계 API 결과값 </summary>

- 연간 접속자 수 결과 화면

<br>

![apiResult0](./img/api-result-0.png)

- 월간 접속자 수 결과 화면

<br>

![apiResult1](./img/api-result-1.png)

- 일간 접속자 수 결과 화면

<br>

![apiResult2](./img/api-result-2.png)

- 평균 하루 로그인 수 결과 화면

<br>

![apiResult3](./img/api-result-3.png)

</details>

<br>

<details> <summary style="color:skyblue"> 최종 API 문서 </summary>

https://brian-jung.gitbook.io/api-docs/eveinformation/eveintroduction

</details>

<br>
