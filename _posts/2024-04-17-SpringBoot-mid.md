---
title: "스프링 부트 중간고사"
excerpt: ""

categories: [SpringBoot]
tags: [SpringBoot, Java, 2024DongyangMiraeUniversity]

toc: true
toc_sticky: true

date: 2024-04-17 22:10:00 +0800
last_modified_at: 2024-04-17 22:20:00 +0800

pin: false
---
###### 프레임워크 장점
- 빠른 구현 시간
    - 개발자는 비지니스 로직만 구현하면 되므로 제한된 시간내에 많은 기능을 구현 가능
- 쉬운 관리
    - 같은 프레임워크가 적용된 어플리케이션은 아키텍쳐가 같으므로 관리가 수월
    - 유지보수의 시간도 절약
- 개발자들의 역량 획일화
- 검증된 아키텍쳐의 재사용과 일관성 유지

###### 스프링 특징
- 경량
    - 여러 개의 모듈로 구성 : 각 모듈은 하나 이상의 JAR파일로 구성
    - 스프링 프레임워크가 POJO(Plain Old Java Object)형태의 객체를 관리하기 때문에 가능
- 제어의 역행 (DI 지원)
    - 자바코드로 하는 것이 아니라 객체 생성을 컨테이너가 대신 처리하기 때문에 소스에 의존관계가 표시되지 않으므로 결합도가 낮아짐
- 관점 지향 프로그래밍
- 컨테이너 역할
    - 특정 객체의 생성과 관리를 담당하여 다양한 기능을 제공

###### MVC 패턴
- Presentation Layer
    - Controller
- Business Layer
    - Service
- Data Access Layer
    - Repository

###### 주요 용어
- IOC (Inversion of Control)
    - 제어의 역전
- AOP (Aspect Oriented Programming)
    - 관점 지향 프로그래밍
- DI (Dependency Injection)
    - 의존성 주입
- PSA (Portable Service Abstraction)
    - 이식 가능한 서비스 추상화
        - 예시) JPA, MyBatis, JDBC

###### 스프링 컨테이너
- 스프링 컨테이너
    - 스프링 안에서 동작하는 빈 생성 및 관리 주체
- 빈
    - 스프링 컨테이너가 생성하고 관리하는 객체

###### 리포지토리 2개 차이점
- CrudRepository
    - 가볍게 사용하기 좋음(Jpa 부모)
- JpaRepository
    - 기능 많이 필요할 때 사용(Crud 자식)

###### 브라우저에서 서버로 데이터를 보내는 
1. https://example.com/users/123
2. https://example.com/users?id=123&name=john
3. URL에 ID를 포함시키고, 요청 본문(request body)에 이름을 포함시켜 서버에 전송하는 방식입니다.
    - URL: https://example.com/users/123
    - 요청 본문: {"name": "john"}

###### 어노테이션

|Annotation|동작|
|--|--|
|@PathValiable|이름 없이 값만 들어올 때 사용|
|@RequestParam|이름 있는 값이 들어올 때 사용|

##### Lombok 추가
- compileOnly 'org.projectlombok:lombok'
- annotationProcessor 'org.projectlombok:lombok'

##### mustache 문법
