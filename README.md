
# Getting Started with Apimatic Calculator

## Introduction

Simple calculator API hosted on APIMATIC

## Install the Package

Install the SDK by adding the following dependency in your project's pom.xml file:

```xml
<dependency>
  <groupId>io.sdks</groupId>
  <artifactId>calculator-java-sdk</artifactId>
  <version>1.2.6</version>
</dependency>
```

You can also view the package at:
https://central.sonatype.com/artifact/io.sdks/calculator-java-sdk/1.2.6

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |

The API client can be initialized as follows:

```java
ApimaticCalculatorClient client = new ApimaticCalculatorClient.Builder()
    .httpClientConfig(configBuilder -> configBuilder
            .timeout(0))
    .environment(Environment.PRODUCTION)
    .build();
```

## List of APIs

* [Simple Calculator](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/controllers/simple-calculator.md)

## SDK Infrastructure

### Configuration

* [Configuration Interface](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/configuration-interface.md)
* [HttpClientConfiguration](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/http-client-configuration-builder.md)

### HTTP

* [Headers](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/headers.md)
* [HttpCallback Interface](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/http-callback-interface.md)
* [HttpContext](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/http-context.md)
* [HttpBodyRequest](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/http-body-request.md)
* [HttpRequest](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/http-request.md)
* [HttpResponse](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/http-string-response.md)

### Utilities

* [ApiException](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/api-exception.md)
* [ApiHelper](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/api-helper.md)
* [FileWrapper](https://www.github.com/Syed-Subtain/calculator-java-java-sdk/tree/1.2.6/doc/file-wrapper.md)

