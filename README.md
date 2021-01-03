# Knowledge List

1. [Software development](#1-software-development)
2. [Data sciense / Machine learning](#2-data-sciense--machine-learning)
3. [Databases](#3-databases)
4. [Security](#4-security)
5. [Cloud platforms](#5-cloud-platforms)
6. [Techdocs](#6-techdocs)
7. [Finance](#7-finance)
8. [Articles](#8-articles)
9. [Monitoring](#9-monitoring)
10. [DevOps](#10-devops)
11. [Company's dev blogs](#11-companys-dev-blogs)
12. [IoT](#12-iot)
13. [Hardware](#13-hardware)

## 1. Software development

### 1.1 Architecture

#### 1.1.1 Onion

* [The Onion Architecture](http://jeffreypalermo.com/blog/the-onion-architecture-part-1/)

#### 1.1.2 Hexagonal

* [Hexagonal Architecture](http://fideloper.com/hexagonal-architecture)

#### 1.1.3 Clean

* [The Clean Architecture from 8thlight](https://8thlight.com/blog/uncle-bob/2012/08/13/the-clean-architecture.html)

#### 1.1.4 Manifests

* [The Twelve-Factor App](https://www.12factor.net)
* [The Reactive Manifesto](https://www.reactivemanifesto.org)
* The API Mandate by Jeff Bezos
  * All teams will henceforth expose their data and functionality
through service interfaces.
  * Teams must communicate with each other through these
interfaces.
  * There will be no other form of interprocess communication
allowed: no direct linking, no direct reads of another team's data
store, no shared-memory model, no back-doors whatsoever. The
only communication allowed is via service interface calls over the
network.
  * It doesn't matter what technology they use. HTTP, Corba,
Pubsub, custom protocols -- doesn't matter. Bezos doesn't care.
  * All service interfaces, without exception, must be designed from
the ground up to be externalizable. That is to say, the team must
plan and design to be able to expose the interface to developers
in the outside world. No exceptions.
  * Anyone who doesn't do this will be fired.
  * Thank you; have a nice day!

### 1.2 Principles

#### 1.2.1 SOLID

* SRP: Single responsibility principle
* OCP: Open/closed principle
* LSP: Liskov substitution principle
* ISP: Interface segregation principle
* DIP: Dependency inversion principle

#### 1.2.2 Law of Demeter: principle of least knowledge

* [Wikipedia](https://en.wikipedia.org/wiki/Law_of_Demeter)

#### 1.2.3 DRY: Don't repeat yoyrself

* [Wikipedia](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)

#### 1.2.4 SSOT: Single source of truth

* [Wikipedia](https://en.wikipedia.org/wiki/Single_source_of_truth)

#### 1.2.5 CQRS: Command Query Responsibility Segregation

* [Command Query Separation from Martin Fowler](https://martinfowler.com/bliki/CommandQuerySeparation.html)
* [Some questions about the command bus](https://matthiasnoback.nl/2015/01/some-questions-about-the-command-bus/)

#### 1.2.6 Event sourcing

* Articles
  * [Event Sourcing from Martin Fowler](https://martinfowler.com/eaaDev/EventSourcing.html)
* Soft
  * [prooph](http://getprooph.org) - CQRS and EventSourcing Infrastructure for PHP


### 1.3 Programming paradigm

* Imperative
  * Object-oriented
  * Procedural
* Declarative
  * Functional

Articles:

* [Wikipedia](https://en.wikipedia.org/wiki/Programming_paradigm)

### 1.4 Concurrency

* [Concurrency in PHP](https://github.com/sokil/php-concurrency-labs)

### 1.5 Patterns

#### Articles

* [(ru) Шаблоны проектирования с человеческим лицом](https://habrahabr.ru/company/mailru/blog/325492/)

### 1.6 Message bus

* Servers
  * Gearman
  * RabbitMQ
    * Durability
    * Excchanges: direct, fanout, topic, headers
    * Cli tools: rabbitmqadmin
  * [ZeroMQ](https://github.com/mkoppanen/php-zmq)
  * Kafka
* Libraries
  * [bernard](https://bernard.readthedocs.io) - Multi-backend PHP library for creating background jobs for later processing
* Articles
  * [(ru)RabbitMQ против Kafka: два разных подхода к обмену сообщениями](https://habr.com/company/itsumma/blog/416629/)

### 1.7 Cache

* [Consistent Hashing: Algorithmic Tradeoffs](https://medium.com/@dgryski/consistent-hashing-algorithmic-tradeoffs-ef6b8e2fcae8)

### 1.8 Search engines

* [Elasticsearch](https://www.elastic.co)

### 1.9 Auth

* oAuth
  * Articles
    * [OAuth2 in 8 Steps (screencast)](http://knpuniversity.com/screencast/oauth)
  * Soft
    * Symfony (PHP)
      * [KnpUOAuth2ClientBundle: Easily talk to an OAuth2 server for social functionality in Symfony (PHP)](https://github.com/knpuniversity/oauth2-client-bundle)
      * [HWIOauthBundle: Symfony2 Facebook and Google Login: The Easy Way (PHP)](http://intelligentbee.com/blog/2015/11/13/symfony2-facebook-google-login/)
* SAML
* LDAP

### 1.10 RPC

* [gRPC](https://grpc.io)
* [JSON-RPC](https://www.jsonrpc.org/specification)
* GraphQL
* REST
  * [Architectural Styles and the Design of Network-based Software Architectures / Roy Thomas Fielding](https://www.ics.uci.edu/~fielding/pubs/dissertation/top.htm)
  * [Problem Details for HTTP APIs](https://tools.ietf.org/html/rfc7807) - This document defines a "problem detail" as a way to carry machine-readable details of errors in a HTTP response to avoid the need to define new error response formats for HTTP APIs.
* Protobuf
* Thrift

### 1.11 Server push

#### Techniques

* WebSocket
* [Server-Sent Events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events)
* Long pooling

#### Implementations

* http://socket.io/ - frontend and backend (node.js) library
* [Faye](https://faye.jcoglan.com) - publish-subscribe messaging system based on the Bayeux protocol. It provides message servers for Node.js and Ruby, and clients for use on the server and in all major web browsers.
* Nginx modules:
  * [nchan](https://nchan.io)
  * [Nginx Push Stream Module](https://github.com/wandenberg/nginx-push-stream-module)

### 1.12 Testing

#### 1.12.1 Unit testing

* PHP
  * [PHPSpec](https://www.phpspec.net/) - A php toolset to drive emergent design by specification
  * [Codeception](https://codeception.com)
  * [Mockery](http://docs.mockery.io/en/latest/) - Simple yet flexible PHP mock object framework for use in unit testing with PHPUnit, PHPSpec or any other testing framework.

### 1.13 Web protocols

* HTTP/2 + SPDY
* [HTTP/2 Server Push (ru)](https://habr.com/en/company/badoo/blog/329722/)

### 1.14 Distributed computing

* Scalability
  * [The Patterns Behind Scalable, Reliable, and Performant Large-Scale Systems](https://github.com/binhnguyennus/awesome-scalability)
* [RAFT: Leader election](https://raft.github.io/)
* [Gossip protocol](https://en.wikipedia.org/wiki/Gossip_protocol)
* [Eventual consistency](https://en.wikipedia.org/wiki/Eventual_consistency)
* [Distributed transactions](https://developers.redhat.com/blog/2018/10/01/patterns-for-distributed-transactions-within-a-microservices-architecture/)
* [Two phase commit](https://en.wikipedia.org/wiki/Two-phase_commit_protocol)

## 2. Data sciense / Machine learning

### 2.1 Common languages, tools and platforms

* [R](https://www.r-project.org/)
* Python libs
  * numpy
  * scikit-learn
  * scipy
  * pyplot
* [CUDA](https://developer.nvidia.com/how-to-cuda-c-cpp)
* [Google AI Project](https://ai.google)
    
### 2.2 Machine learning

* Distributed Random Forest (DRF)
* Generalized Linear Model (GLM)
* Naive Bayes Classifier
* Stacked Ensembles
* Gradient boosting
  * [Wikipedia](https://en.wikipedia.org/wiki/Gradient_boosting)
  * [xgboost](https://github.com/dmlc/xgboost) - Scalable, Portable and Distributed Gradient Boosting (GBDT, GBRT or GBM) Library, for Python, R, Java, Scala, C++ and more. Runs on single machine, Hadoop, Spark, Flink and DataFlow
* [Unbalanced data dealing](https://shiring.github.io/machine_learning/2017/04/02/unbalanced)

### 2.3 Deep learning / Neural networks

Tools:
  * [Tensorflow](https://www.tensorflow.org/)
  * [Keras](https://keras.io) - high-level neural networks API, capable of running on top of TensorFlow, CNTK, or Theano.
  
### 2.4 OCR

* [Tesseract OCR](https://github.com/tesseract-ocr/)
* [OpenCV](https://opencv.org)

### 2.5 Conversational AI / Natural-language processing

Conversational AI:
* [Rasa - Conversational AI](https://rasa.com)
* [Haptik - Conversational AI](https://haptik.ai/)
* [Recast - The collaborative platform to build, train, deploy and monitor intelligent bots for developers Or with your email](https://recast.ai)
* [Google DialogFlow](https://dialogflow.com)
  * [DialogFlow Fulfillment](https://github.com/dialogflow/dialogflow-fulfillment-nodejs)
  * [DialogFlow PHP SDK](https://github.com/GoogleCloudPlatform/google-cloud-php-dialogflow)
* [Microsoft LUIS](https://www.luis.ai)
* [Microsoft Bot Framework](https://dev.botframework.com)
* [Amazon Lex](https://aws.amazon.com/lex/)
* [Facebook Wit.ai](https://wit.ai)
* [IBM Watson](https://www.ibm.com/watson/services/natural-language-understanding/)

Bot frameworks:
* [Botpress](https://botpress.io)
* [Botman](https://botman.io)
* [SuperScriptJS](http://superscriptjs.com)

Articles:
* [Google AI](https://ai.google/research/teams/nlu/)
* [Natural language processing, NLP](https://en.wikipedia.org/wiki/Natural_language_processing)
* [Natural language understanding, NLU](https://en.wikipedia.org/wiki/Natural_language_understanding)


### 2.6 Visualization

* Tableau
* Periscope Data
* Looker
* jupyter notebook

## 3. Databases

### 3.1 Theory

#### 3.1.1 CAP: Consistency, Availability, Partition tolerance

* [Wikipedia](https://en.wikipedia.org/wiki/CAP_theorem)

#### 3.1.2 ACID: Atomicity, Consistency, Isolation, Durability

In contrast to BASE.

* [Wikipedia](https://en.wikipedia.org/wiki/ACID)

#### 3.1.3 BASE: Basically Available, Soft state, Eventual consistency

In contrast to ACID.

* [Eventual consistency](https://en.wikipedia.org/wiki/Eventual_consistency)

#### 3.1.3 MVCC: Multiversion concurrency control

* [Wikipedia](https://en.wikipedia.org/wiki/Multiversion_concurrency_control)

#### 3.1.5 ETL: Extract, transform, load

* [Wikipedia](https://en.wikipedia.org/wiki/Extract,_transform,_load)

### 3.2 Normlization

### 3.3 Joins

* [Infographic](http://www.codeproject.com/KB/database/Visual_SQL_Joins/Visual_SQL_JOINS_orig.jpg)

### 3.4 Partitions

### 3.5 Triggers

### 3.6 Indexes

### 3.7 Storage

* Row-based
* Column-based
* NoSQL
  * Document-based
  * Key-value
  * Column
  * Graph
  
### 3.8 Processing

#### 3.8.1 OLTP: On-line Transaction Processing

#### 3.8.2 OLAP: On-line Analytical Processing

### 3.9 Database scema migration

* http://www.liquibase.org/
* https://www.percona.com/doc/percona-toolkit/LATEST/pt-online-schema-change.html

### 3.10 Articles and tutorials

* [How Does a Database Work?](https://cstack.github.io/db_tutorial/)

## 4. Security

### 4.1 Cryptography

### 4.2 XSS

### 4.3 CSRF

### 4.4 SQL injection

## 5. Cloud platforms

### 5.1 Amazon Web Services

* [localstack](https://localstack.cloud) - Develop and test your cloud apps offline.

### 5.2 Microsoft Azure

### 5.3 Google Cloud

* [Cloud](https://cloud.google.com)
  * [A local emulator for Google Cloud Functions](https://github.com/GoogleCloudPlatform/cloud-functions-emulator) - allows you to deploy, run, and debug your Cloud Functions on your local machine before deploying them to the production Google Cloud Functions service.
* [Firebase](https://firebase.google.com)

### 5.4 Corezoid

* [Official site](https://new.corezoid.com)

## 6. Techdocs

### 6.1 Static site generator

* [Jekyll](https://jekyllrb.com/docs/structure/)
* [Docusaurus](https://docusaurus.io) - Easy to Maintain Open Source Documentation Websites

### 6.2 API dods

* [RAML](https://raml.org) - RESTful API Modeling Language (RAML) makes it easy to manage the whole API lifecycle from design to sharing. It's concise - you only write what you need to define - and reusable. It is machine readable API design that is actually human friendly.
* [Swagger](https://swagger.io) - Design is the foundation of your API development. Swagger makes API design a breeze, with easy-to-use tools for developers, architects, and product owners.

## 7. Finance

* [Shamir's Secret Sharing](https://en.wikipedia.org/wiki/Shamir%27s_Secret_Sharing)

## 8. Articles

* [Web developer roadmap (frontend, backend, devops)](https://github.com/kamranahmedse/developer-roadmap)

## 9. Monitoring

### 9.1 Logging

#### Tools

* ELK
  * [Curator](https://github.com/elastic/curator)
* Rsyslogd

#### Usecases

* [(ru) Работа с потоком логов в реальном времени с помощью Heka. Опыт Яндекс.Денег](https://habr.com/company/yamoney/blog/328018/)
* [(ru) Сбор и анализ логов демонов в Badoo](https://habr.com/company/badoo/blog/280606/)

### 9.2 Monitoring

#### Tools

* [Pinba](http://pinba.org) - MySQL storage engine that acts as a realtime monitoring/statistics server for PHP using MySQL as a read-only interface.
* StatsD + Graphite
* [InfluxDB](https://www.influxdata.com) - Time Series Platform
* [prometheus](https://prometheus.io/)
* [fluentd](https://www.fluentd.org)

#### Usecases

* [(ru) Обзор систем мониторинга серверов. Заменяем munin на…](https://habr.com/post/331016/)
* [(ru) Истории успеха Kubernetes в production. Часть 4: SoundCloud (авторы Prometheus)](https://habr.com/company/flant/blog/339724/)

## 10. DevOps

* Infrastructure automation
  * Ansible
  * Puppet
  * Chef
  * Capistrano
* Process management:
  * [supervisord](http://supervisord.org/)
  * [mmonit](https://mmonit.com/)
* HashiCorp
  * Consul
    * [Conful templte](https://github.com/hashicorp/consul-template)
    * [Scratch](http://gohugo.io/functions/scratch/) - for consul templating
  * Vault

## 11. Company's dev blogs

* [Riot Games](https://engineering.riotgames.com)
* [GitHub](https://developer.github.com)
* [Uber](https://eng.uber.com/)
* [Haptik](https://haptik.ai/tech/)

## 12. IoT

### 12.1 MQTT: Message Queuing Telemetry Transport

* Soft
  * [Eclipse Mosquitto™ - An open source MQTT broker](https://mosquitto.org)
  * [Intel IoT Code Samples](https://software.intel.com/iot/documentation/code-samples)
* Articles
  * [Wiki](https://en.wikipedia.org/wiki/MQTT)
  * [(ru) ESP8266 в качестве MQTT брокера для мобильного приложения](https://habr.com/post/326794/)
  * (ru) Как построить IIoT архитектуру своими руками
    * [Part 1](https://habr.com/company/itsumma/blog/415933/)
    * [Part 2](https://habr.com/company/itsumma/blog/416291/)

### 12.2 Network management

* ThingsBoard
  * https://github.com/thingsboard/thingsboard
* NiFi
  * Sort
    * [NiFi: An easy to use, powerful, and reliable system to process and distribute data](https://nifi.apache.org)
    * [MiNiFi: A subproject of Apache NiFi to collect data where it originates](https://nifi.apache.org/minifi/)
  * Articles
    * [(ru) Как построить IIoT архитектуру своими руками](https://habr.com/company/itsumma/blog/415933/)

## 13. Hardware

### 13.1 GSM / Radio

* [Scan for GSM base stations in a given frequency band and can use those GSM base stations to calculate the local oscillator frequency offset](https://github.com/steve-m/kalibrate-rtl)
* [RTL SDR](http://www.rtl-sdr.com/rtl-sdr-quick-start-guide/)
* [Радиоприёмник из DVB стика за $8 — изучаем SDR с GNURadio](https://habr.com/en/company/zwave/blog/390421/)
* [«Заводим» радиоуправляемые розетки без пульта](https://habr.com/en/post/212215/)
* [Зубочистка-детектив раскрывает секрет радиопротокола](https://habr.com/en/post/211594/)
* [Dump 1090 is a Mode S decoder specifically designed for RTLSDR devices](https://github.com/antirez/dump1090)
* [ADS-B Decoding Guide](http://adsb-decode-guide.readthedocs.io/en/latest/)
* [Software to turn the RTL2832U into an SDR](https://github.com/steve-m/librtlsdr)
* [GNU Radio / HackRF One](https://habrahabr.ru/post/325894/)
* [Introduction to Radar Systems](https://www.ll.mit.edu/outreach/introduction-radar-systems)
* [A WebSDR is a Software-Defined Radio receiver connected to the internet, allowing many listeners to listen and tune it simultaneously](http://www.websdr.org/)

### 13.2 ESP8266

* [(ru) О вкусном и здоровом питании ESP8266 от батареек](https://habr.com/post/304936/)
