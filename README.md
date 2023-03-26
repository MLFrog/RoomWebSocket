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

----

## 테스트 및 검증 필요

1. 채팅 서버를 먼저 구현하여 정상적인 Room 생성이 이뤄지는지 확인 필요  
2. Room Key 값 생성 및 관리 주체는 어떤 서버로 해야하는가 심도 깊은 고민 필요  