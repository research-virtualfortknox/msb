
<p align="center">
  <a href="https://research.virtualfortknox.de" target="_blank" rel="noopener noreferrer">
    <img src="https://research.virtualfortknox.de/static/cms/img/vfk_research_logo.png" alt="VFK Research Logo" height="70" >
  </a>
</p>

# Manufacturing Service Bus

The Manufacturing Service Bus (MSB) is an integration platform based on a software-oriented architecture. It enables fast and low-effort integration of smart objects (e.g. IoT devices, shopfloor machinery) and applications (e.g. database, dashboard). The MSB offers connectivity via various communication protocols such as RESTful Web Service or WebSocket API and various communication standards, for example OPC UA or MQTT. The actual integration of the connected smart objects and applications takes place via configurable connections, so-called integration flows, which can contain additional logic.

![Field of application](doc/images/field_of_application.png)

## Get started

Follow the instructions to [setup a Docker-based instance of the MSB](.docker-compose/README.md) for testing and evaluation purposes.

To connect smart objects or applications, there are various client libraries and integrations available from which you can choose the one that best fits to your use case.

| Language   | Client library                                                                                         |
|------------|--------------------------------------------------------------------------------------------------------|
| Java       | [msb.client.websocket.java](https://github.com/research-virtualfortknox/msb-client-websocket-java)     |
| Python     | [msb.client.websocket.python](https://github.com/research-virtualfortknox/msb-client-websocket-python) |
| Node.js    | [msb.client.websocket.nodejs](https://github.com/research-virtualfortknox/msb-client-websocket-nodejs) |
| C          | [msb.client.websocket.c](https://github.com/research-virtualfortknox/msb-client-websocket-c)           |
| C++        | [msb.client.websocket.c](https://github.com/research-virtualfortknox/msb-client-websocket-c)           |
| C #        | [msb.client.websocket.csharp](https://github.com/research-virtualfortknox/msb-client-websocket-csharp) |
| Node-Red   | [node-red-contrib-msb](https://github.com/research-virtualfortknox/node-red-contrib-msb)               |

The connection to a Restful-based web service can be configured, which is supported by a wizard in the UI.

## Websites

- https://virtualfortknox.de/ (Official website)
- https://research.virtualfortknox.de/ (Official research website)
- https://github.com/research-virtualfortknox/msb (source code and issue tracker)

## Copyright & License

Copyright (c) 2012-2024 Fraunhofer IPA. This file is part of the Manufacturing Service Bus (MSB) open source project, which is dedicated to providing the middleware for test and evaluation purposes.

The provided parts of the Manufacturing Service Bus (MSB) are free software: You may redistribute and/or modify them under the terms of the GNU Lesser General Public License as published by the Free Software Foundation, either version 3 of the License or (at your option) any later version.

The provided parts of the Manufacturing Service Bus (MSB) is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.

You should have received a copy of the GNU Lesser General Public License along with Manufacturing Service Bus. If not, see http://www.gnu.org/licenses/.

To publish a commercial product that uses Manufacturing Service Bus or to use Manufacturing Service Bus productively, commercial licenses and support are also available: Contact info@virtualfortknox.de for more information.