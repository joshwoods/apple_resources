

- SMS and Call Reporting
-  ILMessageFilterQueryHandling 

Protocol

# ILMessageFilterQueryHandling

A set of methods implemented by a Message Filter app extension to handle query requests.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
protocol ILMessageFilterQueryHandling : NSObjectProtocol
```

## Mentioned in 

Creating a Message Filter App Extension

## Overview

A Message Filter app extension that adopts this protocol forms a response about the message described in the query, based on information that it either stores locally or receives from an associated network service.

When the app extension defers a query request to a server, the system handles all network communication, passing the request to the server and passing the server’s response back to the app extension.

## Topics

### Handling a Query Request

func handle(ILMessageFilterQueryRequest, context: ILMessageFilterExtensionContext, completion: (ILMessageFilterQueryResponse) -> Void)

Evaluates a query request and tells the system how to handle the message represented in the request.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Queries

class ILMessageFilterQueryRequest

A request for a Message Filter app extension to determine the status of a message received from an unknown sender.

