# Back-end-Develop-Practice

## 1st Assignment

<br>

Eclipse, Spring 설치

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

<br>

<details> <summary style="color:skyblue"> API 문서 초안 작성 </summary>

https://brian-jung.gitbook.io/api-docs/eveinformation/eveintroduction

</details>

<br>

## 3st Assignment

<br>

스프링부트 개발 환경 설정하기

<details> <summary style="color:skyblue"> 프로젝트 세팅 완료 </summary>

![SpringBoot0](./img/springboot-start_1.png)

![SpringBoot1](./img/springboot-start_2.png)

![SpringBoot2](./img/springboot-start.png)

</details>

<br>

<details> <summary style="color:skyblue"> Pom.xml 수정 완료 </summary>

![BootPOM0](./img/boot-pom_1.png)

![BootPOM1](./img/boot-pom_2.png)

![BootPOM2](./img/boot-pom_3.png)

</details>

<br>

<details> <summary style="color:skyblue"> application.properties 수정 완료 </summary>

![AppPP0](./img/app-properties_1.png)

![AppPP1](./img/app-properties_2.png)

</details>

<br>

<details> <summary style="color:skyblue"> 기본 TEST </summary>

![TEST0](./img/boot-test_1.png)

![TEST1](./img/boot-test_2.png)

![TEST2](./img/boot-test_3.png)

![TEST3](./img/boot-test_4.png)

</details>

<br>

<details> <summary style="color:skyblue"> 통계(SW활용현황) API를 위한 DB, TABLE 생성 </summary>

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