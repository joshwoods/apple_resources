

- Foundation
- URLProtocol
-  canInit(with:) 

Type Method

# canInit(with:)

Determines whether the protocol subclass can handle the specified task.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func canInit(with task: URLSessionTask) -> Bool
```

## Parameters 

`task`  

A URL session task containing the request to be handled.

## Discussion

A subclass should inspect the task’s request and determine whether or not the implementation can perform a load with that task.

This is an abstract method and subclasses must provide an implementation.

## See Also

### Determining If a subclass can handle a request

class func canInit(with: URLRequest) -> Bool

Determines whether the protocol subclass can handle the specified request.

