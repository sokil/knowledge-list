# Knowledge List


1. [Software development](#1-software-development)
2. [Data sciense](#2-data-sciense)
3. [Databases](#3-databases)
4. [Security](#4-security)
5. [Cloud platforms](#5-cloud-platforms)
6. [Techdocs](#6-techdocs)
7. [Finance](#7-finance)
8. [Articles](#8-articles)

## 1. Software development

### 1.1 Architecture

#### 1.1.1 Onion

* [The Onion Architecture](http://jeffreypalermo.com/blog/the-onion-architecture-part-1/)

#### 1.1.2 Hexagonal

* [Hexagonal Architecture](http://fideloper.com/hexagonal-architecture))

#### 1.1.3 Clean

* [The Clean Architecture from 8thlight](https://8thlight.com/blog/uncle-bob/2012/08/13/the-clean-architecture.html)

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

### 1.6 Message bus

* Gearman
* RabbitMQ
  * Durability
  * Excchanges: direct, fanout, topic, headers
  * Cli tools: rabbitmqadmin
* [ZeroMQ](https://github.com/mkoppanen/php-zmq)
* Kafka

### 1.7 Cache

* [Consistent Hashing: Algorithmic Tradeoffs](https://medium.com/@dgryski/consistent-hashing-algorithmic-tradeoffs-ef6b8e2fcae8)

### 1.8 Search engines

* [Elasticsearch](https://www.elastic.co)

### 1.9 Auth

* oAuth
* SAML
* LDAP

### 1.10 RPC

* [gRPC](https://grpc.io)
* GraphQL
* REST
  * [Architectural Styles and the Design of Network-based Software Architectures / Roy Thomas Fielding](https://www.ics.uci.edu/~fielding/pubs/dissertation/top.htm)
  * [Problem Details for HTTP APIs](https://tools.ietf.org/html/rfc7807) - This document defines a "problem detail" as a way to carry machine-readable details of errors in a HTTP response to avoid the need to define new error response formats for HTTP APIs.

### 1.11 Server push

* WebSocket
* [Server-Sent Events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events)
* Long pooling

## 2. Data sciense

### 2.1 Common languages, tools and platforms

* [R](https://www.r-project.org/)
* Python libs
  * numpy
  * scikit-learn
  * scipy
  * pyplot
* [CUDA](https://developer.nvidia.com/how-to-cuda-c-cpp)
* Deep Learning / Neural networks
  * [Tensorflow](https://www.tensorflow.org/)
  * [Keras](https://keras.io) - high-level neural networks API, capable of running on top of TensorFlow, CNTK, or Theano.
    
### 2.2 Machine learning

* Distributed Random Forest (DRF)
* Generalized Linear Model (GLM)
* Naive Bayes Classifier
* Stacked Ensembles
* Gradient boosting
  * [Wikipedia](https://en.wikipedia.org/wiki/Gradient_boosting)
  * [xgboost](https://github.com/dmlc/xgboost) - Scalable, Portable and Distributed Gradient Boosting (GBDT, GBRT or GBM) Library, for Python, R, Java, Scala, C++ and more. Runs on single machine, Hadoop, Spark, Flink and DataFlow
* [Unbalanced data dealing](https://shiring.github.io/machine_learning/2017/04/02/unbalanced)

### 2.3 OCR

* [Tesseract OCR](https://github.com/tesseract-ocr/)
* [OpenCV](https://opencv.org)

### 2.4 Visualization

* Tableau
* Periscope Data
* Looker
* jupyter notebook

## 3. Databases

### 3.1 Theory

#### 3.1.1 CAP: Consistency, Availability, Partition tolerance

* [Wikipedia](https://en.wikipedia.org/wiki/CAP_theorem)

#### 3.1.2 ACID: Atomicity, Consistency, Isolation, Durability

* [Wikipedia](https://en.wikipedia.org/wiki/ACID)

#### 3.1.3 MVCC - Multiversion concurrency control

* [Wikipedia](https://en.wikipedia.org/wiki/Multiversion_concurrency_control)

### 3.2 Normlization

### 3.3 Joins

* [Infographic](http://www.codeproject.com/KB/database/Visual_SQL_Joins/Visual_SQL_JOINS_orig.jpg)

### 3.4 Partitions

### 3.5 Triggers

### Database scema migration

* http://www.liquibase.org/
* https://www.percona.com/doc/percona-toolkit/LATEST/pt-online-schema-change.html

## 4. Security

### 4.1 XSS

### 4.2 CSRF

### 4.3 SQL injection

## 5. Cloud platforms

## 6. Techdocs

### 6.1 Static site generator

* [Jekyll](https://jekyllrb.com/docs/structure/)

## 7. Finance

* [Shamir's Secret Sharing](https://en.wikipedia.org/wiki/Shamir%27s_Secret_Sharing)

## 8. Articles

* [Web developer roadmap (frontend, backend, devops)](https://github.com/kamranahmedse/developer-roadmap)
