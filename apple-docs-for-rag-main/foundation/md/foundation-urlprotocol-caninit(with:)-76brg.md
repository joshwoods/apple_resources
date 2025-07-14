

- Foundation
- URLProtocol
-  canInit(with:) 

Type Method

# canInit(with:)

Determines whether the protocol subclass can handle the specified request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func canInit(with request: URLRequest) -> Bool
```

## Parameters 

`request`  

The request to be handled.

## Return Value

true if the protocol subclass can handle `request`, otherwise false.

## Discussion

A subclass should inspect `request` and determine whether or not the implementation can perform a load with that request.

This is an abstract method and subclasses must provide an implementation.

## See Also

### Determining If a subclass can handle a request

class func canInit(with: URLSessionTask) -> Bool

Determines whether the protocol subclass can handle the specified task.

