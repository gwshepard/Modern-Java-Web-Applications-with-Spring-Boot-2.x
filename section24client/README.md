# org.packt.springboot22

Farm Management REST WS
- API version: 1.0-SNAPSHOT
  - Build date: 2019-09-01T10:47:23.730+08:00

The web service layer.


*Automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen)*


## Requirements

Building the API client library requires:
1. Java 1.7+
2. Maven/Gradle

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn clean install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn clean deploy
```

Refer to the [OSSRH Guide](http://central.sonatype.org/pages/ossrh-guide.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
  <groupId>section24</groupId>
  <artifactId>org.packt.springboot22</artifactId>
  <version>1.0.0</version>
  <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
compile "section24:org.packt.springboot22:1.0.0"
```

### Others

At first generate the JAR by executing:

```shell
mvn clean package
```

Then manually install the following JARs:

* `target/org.packt.springboot22-1.0.0.jar`
* `target/lib/*.jar`

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

```java

import org.packt.springboot22.vid02.config.*;
import org.packt.springboot22.vid02.config.auth.*;
import org.packt.springboot22.vid02.model.*;
import org.packt.springboot22.vid02.client.SignupControllerApi;

import java.io.File;
import java.util.*;

public class SignupControllerApiExample {

    public static void main(String[] args) {
        
        SignupControllerApi apiInstance = new SignupControllerApi();
        Object reqParams = null; // Object | reqParams
        try {
            String result = apiInstance.addNewFormSignupUsingPOST(reqParams);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling SignupControllerApi#addNewFormSignupUsingPOST");
            e.printStackTrace();
        }
    }
}

```

## Documentation for API Endpoints

All URIs are relative to *https://localhost:8082/farmservice*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*SignupControllerApi* | [**addNewFormSignupUsingPOST**](docs/SignupControllerApi.md#addNewFormSignupUsingPOST) | **POST** /signup/user/add/form | Add new user.
*SignupControllerApi* | [**addNewSignupUsingPOST**](docs/SignupControllerApi.md#addNewSignupUsingPOST) | **POST** /signup/user/add | Add new user.
*SignupControllerApi* | [**deleteSignupUsingDELETE**](docs/SignupControllerApi.md#deleteSignupUsingDELETE) | **DELETE** /signup/user/delete/{username} | Delete user account.
*SignupControllerApi* | [**getApprovedUsersUsingGET**](docs/SignupControllerApi.md#getApprovedUsersUsingGET) | **GET** /signup/users/approved | Returns all approved users only.
*SignupControllerApi* | [**getSignedupUserUsingGET**](docs/SignupControllerApi.md#getSignedupUserUsingGET) | **GET** /signup/users/{username} | Returns users with matched username.
*SignupControllerApi* | [**getSignedupUsersUsingGET**](docs/SignupControllerApi.md#getSignedupUsersUsingGET) | **GET** /signup/users | Returns all users.
*SignupControllerApi* | [**getTotalUsersUsingGET**](docs/SignupControllerApi.md#getTotalUsersUsingGET) | **GET** /signup/users/count | Returns total number of users.
*SignupControllerApi* | [**partialupdateSignupUsingPATCH**](docs/SignupControllerApi.md#partialupdateSignupUsingPATCH) | **PATCH** /signup/user/update/partial/{username} | Update some profile detail.
*SignupControllerApi* | [**updateSignupUsingPUT**](docs/SignupControllerApi.md#updateSignupUsingPUT) | **PUT** /signup/user/update/full/{username} | Update a user account.


## Documentation for Models

 - [ProfileInformation](docs/ProfileInformation.md)


## Documentation for Authorization

All endpoints do not require authorization.
Authentication schemes defined for the API:

## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author



