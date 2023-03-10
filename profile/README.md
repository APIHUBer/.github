<p align="center">
  <img src="https://cs410032002121be004.blob.core.windows.net/icon/logo.svg" width="250" />
</p>

## Introduction
> `APIHUB` is an API interface open calling platform based on React(Typescript), Spring Boot, Dubbo, and Gateway. Administrators can integrate and release APIs, visualize the usage of each API, and grant access to users for calling APIs, browsing APIs, and online debugging. Users can easily call APIs through a client SDK.

> According to the business process, the entire backend of the project is divided into 5 sub-projects: web system, simulated interfaces, public modules, client SDK, and API gateway, and managed with Maven for multi-module dependency management and packaging.
> 

- Using the `Ant Design Pro` and a self-built `Spring Boot` project template, the initial web project was quickly constructed, and basic capabilities such as unified permission management and multi-environment switching were implemented for front-end and back-end.

- Flexible queries of the `MySQL` database were implemented using `QueryWrapper` based on the `MyBatis Plus` framework, and back-end CRUD basic code was automatically generated using the `MyBatis X` plugin to reduce repetitive work.

- Using `Swagger` and `Knife4j` automatically generate `OpenAPI` specification interface documents. On this basis, the front-end used plugins to automatically generate interface request code, reducing the cost of front-end and back-end cooperation.

- To prevent malicious API calls, an `API signature authentication algorithm` was designed to authenticate users and assign them unique ak/sk to ensure call security and traceability (i.e., to facilitate the statistics of API call times).

- To solve the problem of high development costs for developers (having to use HTTP and signature encapsulation to call interfaces, an average of about 20 lines of code), a `client SDK` was developed based on `Spring Boot Starter`, allowing API calls with just one line of code, improving the development experience.

- Front-end: Using the ECharts (or AntV) visualization library, analysis charts (such as pie charts) were implemented for API calls, and the loading configuration was used to improve the loading experience.

- `Spring Cloud Gateway` was chosen as the `API gateway` to implement `routing forwarding`, `access control,`, and to centrally `handle signature verification`, `request parameter verification`, `API call statistics`, and other business logic, improving security and facilitating system development and maintenance.


## Technologies

### Frontend
- React
- TypeScript
- [Ant Design Pro](https://pro.ant.design/)
- [Ant Design Procomponents](https://procomponents.ant.design/en-US)
- [Umi](https://github.com/umijs/umi)

### Backend
- Java Spring Boot
- Spring Boot Starter(SDK Development)
-

## processing...