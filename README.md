# Room WebSocket Server

InfraStructure PreView
----
Spring Boot: Spring Boot를 사용하여 사용자 인증, 메시지 지속성 및 메시지 전달을 처리하는 백엔드 애플리케이션을 만듭니다.

Spring WebFlux: Spring WebFlux를 사용하여 클라이언트와 서버 간의 WebSocket 통신을 처리합니다. WebSocketHandler 인터페이스를 사용하여 들어오는 WebSocket 메시지를 처리하기 위한 사용자 지정 핸들러를 구현할 수 있습니다.

RabbitMQ: 클라이언트와 서버 간의 메시지 송수신을 위한 메시지 브로커로 RabbitMQ를 사용합니다. 메시지 전달을 처리하기 위해 RabbitMQ 교환 및 큐를 생성할 수 있습니다.

프런트엔드: React, Vue.js 또는 Angular와 같은 프런트엔드 프레임워크를 사용하여 채팅 시스템용 사용자 인터페이스를 만듭니다. WebSocket API를 사용하여 백엔드 WebSocket 서버에 연결하고 메시지를 주고받습니다.

다음은 인프라를 구현하는 높은 수준의 단계입니다:

Spring WebFlux 및 RabbitMQ 종속성을 사용하여 Spring Boot 프로젝트를 설정합니다.

Spring Security를 사용하여 사용자 인증 시스템을 구현합니다.

메시지 전달을 위한 RabbitMQ 교환 및 큐를 설정합니다.

Spring WebFlux를 사용하여 웹 소켓 핸들러를 구현합니다.

MySQL 또는 MongoDB와 같은 데이터베이스를 사용하여 메시지 지속성을 구현합니다.

React 또는 Vue.js와 같은 JavaScript 프레임워크를 사용하여 프런트엔드 애플리케이션을 만듭니다.

WebSocket API를 사용하여 프런트엔드와 백엔드 간의 WebSocket 통신을 구현합니다.

WebSocket API를 사용하여 프론트엔드에서 메시지 송수신 기능을 구현합니다.

애플리케이션을 테스트하여 메시지가 올바르게 송수신되는지 확인합니다.

Spring Boot, Spring Webflux, Redis 및 RabbitMQ를 사용하여 채팅 시스템을 만들 수 있습니다.

# Redis 추가 version
다음은 가능한 높은 수준의 아키텍처입니다:

클라이언트는 WebSocket을 사용하여 Spring Boot 서버에 메시지를 보냅니다.
서버는 메시지를 수신하여 Redis에 저장한 후 RabbitMQ 토픽 교환에 게시합니다.
구독한 모든 클라이언트는 RabbitMQ를 통해 메시지를 수신합니다.
클라이언트는 웹소켓 연결을 통해 메시지를 수신하고 채팅 창에 메시지를 표시합니다.
인프라를 설정하는 단계는 다음과 같습니다:

채팅 메시지를 저장할 Redis 인스턴스를 설정합니다.
메시지 교환을 처리할 RabbitMQ 인스턴스를 설정합니다.
Spring Boot 프로젝트를 생성하고 다음과 같은 종속성을 추가합니다: spring-boot-starter-webflux, spring-boot-starter-data-redis-reactive, spring-boot-starter-amqp.
클라이언트에서 들어오는 메시지를 수신하고 처리하기 위해 Spring Boot 서버에 WebSocket 엔드포인트를 구현합니다.
채팅 메시지를 저장하고 검색하기 위해 Redis 리포지토리를 구현합니다.
각각 채팅 메시지를 게시하고 수신하기 위해 RabbitMQ 게시자 및 구독자를 구현합니다.

----

## 테스트 및 검증 필요

1. 채팅 서버를 먼저 구현하여 정상적인 Room 생성이 이뤄지는지 확인 필요  
2. Room Key 값 생성 및 관리 주체는 어떤 서버로 해야하는가 심도 깊은 고민 필요  