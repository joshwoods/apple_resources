

- XPC
-  Creating XPC services 

Article

# Creating XPC services

Configure a listener, establish a client session, and exchange messages between processes.

## Overview

XPC services have two sides: a listener or server that receives incoming connections and performs tasks, and a client that initiates connections and makes requests. The service in this example performs a task of adding two numbers together. The sections below show:

- How to configure the listener, or server, and prepare to receive messages

- How the client connects to the listener

- How the client sends a message to the listener and receives a response

### Add an XPC Service target to your project

The XPC Service template provides a starting point for you to build the listener side of an XPC connection. To add a target, follow these steps:

1.  Open your app or framework project in Xcode.

2.  Choose File \> New \> Target.

3.  Select the XPC Service from the Framework & Library section.

4.  Click Next.

5.  Specify the name for the service.

6.  Select Low Level - libXPC for the API Level popup.

7.  Click Finish.

Important

Take note of the bundle identifier value shown in the sheet when you enter the name and API level. Clients use this value to connect to the service.

### Accept incoming connection requests

When `launchd` launches an XPC service, it starts a process that runs the binary of the service. To perform tasks, the service creates an XPCListener with a service name and a closure to handle incoming session requests. For services in an app bundle or framework, the service name is the XPC service’s bundle identifier. After creating an `XPCListener`, the service must call dispatchMain() to begin processing requests.

Each time a client initiates a session with the service, the system invokes the listener’s closure, passing an XPCListener.IncomingSessionRequest. The listener either accepts or rejects the request. If it accepts the incoming request, it provides a request-handling closure to receive the message the client sent. In this example, the service passes that message to a custom method, `performCalculation(with:)`, to perform the task.

```
```

If the listener rejects the request, it provides a `reason` string to inform the client why it rejected the request.

```
```

### Perform a task and respond to messages

After creating the listener and accepting an incoming request, the service is ready to perform its defined task. In the example below, clients submit requests by passing an instance of a custom Codable type named `CalculationRequest`. The request contains two numbers that the service adds together. The service’s response to the request is an instance of `CalculationResponse` that contains the result of the addition.

```
```

The listener’s request-handling closure receives an XPCReceivedMessage parameter that contains the encoded object the client sent. To perform the task, the service decodes the message using the appropriate `CalculationRequest` type. To reply to the client, the service creates an instance of `CalcuationResponse`, populates it with the result of the calculation, and returns it.

```
```

With the connection and request-handling code in place, `launchd` can now hand off client requests to your XPC service.

### Connect from the client to the server and make requests

When a client wants to use an XPC service, it creates a session with the service and then sends it a message. The following code shows how to set up an XPC session. In response to this request, `launchd` locates the service, launching it if necessary, and establishes a connection between the client process and the listener’s process.

```
```

After creating the session, the client can send its request to the service. In the following code, the client creates the `CalculationRequest` with two numbers to add. While the client waits for a synchronous reply, the system sends the message to the service, arriving at the listener’s handler, as shown previously.

```
```

The system encodes the response from the listener in an instance of XPCReceivedMessage. The client decodes the response using the `CalculationResponse` type, and then processes the result.

```
```

## See Also

### Interprocess communication

class XPCListener

A type that performs tasks for clients across process boundaries.

class XPCSession

A type that sends messages to a server process.

struct XPCReceivedMessage

A type that represents a message sent between a session and a listener.

typealias xpc_listener_t

A C type that performs tasks for clients across process boundaries.

typealias xpc_session_t

A C type that sends messages to a server process.

