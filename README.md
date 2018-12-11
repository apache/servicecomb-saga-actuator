# Saga Actuator [![Build Status](https://travis-ci.org/apache/servicecomb-saga-actuator.svg?branch=master)](https://travis-ci.org/apache/servicecomb-saga-actuator?branch=master) [![Coverage Status](https://coveralls.io/repos/github/apache/servicecomb-saga-actuator/badge.svg?branch=master)](https://coveralls.io/github/apache/servicecomb-saga-actuator?branch=master) [![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)

## Purpose
Saga is a type of Compensating Transaction pattern, which provides a simple way to help users solve the data consistency problems encountered in micro-service applications. Saga Actuator provides

## Documentation
Reference documentation is available on the [ServiceComb website](http://servicecomb.io/).

## Major Architecture of Saga
* saga-core(transaction and compensation handling logic)
* saga-core-akka(leverage the actor for executor)
* saga-format(data serialization and deserialization)
* saga-transports(communication protocol implementation such as rest or rpc in the future)
* saga-discovery(service discovery)
* saga-spring(restful service framework)

![Saga](docs/static_files/saga.png)

## Prerequisites
You will need:
1. [Oracle JDK 1.8+](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
2. [Maven 3.x](https://maven.apache.org/install.html)
3. [Docker](https://www.docker.com/get-docker)

## Building
Download the source code.
```
git clone https://github.com/apache/servicecomb-saga-actuator
```

Enter the Saga root directory,biuld Saga project by maven command and generate a docker image named saga-spring in local.
```
mvn package -DskipTests -Pdocker
```

## Reference API
See [Saga API](docs/api/api.md) for details.


## Example
See [Saga demo](saga-demo/README.md) for details.

## Contact
* [issues](https://issues.apache.org/jira/browse/SCB)
* [gitter](https://gitter.im/ServiceCombUsers/Saga)
* mailing list: [subscribe](mailto:dev-subscribe@servicecomb.apache.org) [view](https://lists.apache.org/list.html?dev@servicecomb.apache.org)

## Contributing
See [Pull Request Guide](http://servicecomb.io/developers/pull-request-guide/) for details.

## Reporting Issues
See reporting bugs for details about reporting any issues.
