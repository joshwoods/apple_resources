

- Foundation
- NSURLConnection
-  canHandle(\_:) 

Type Method

# canHandle(\_:)

Returns whether a request can be handled based on a preflight evaluation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func canHandle(_ request: URLRequest) -> Bool
```

## Parameters 

`request`  

The request to evaluate. The connection deep-copies the request on creation.

## Return Value

true if a preflight operation determines that a connection with `request` can be created and the associated I/O can be started, false otherwise.

## Discussion

The result of this method is valid as long as no URLProtocol classes are registered or unregistered, and `request` remains unchanged. Applications should be prepared to handle failures even if they have performed request preflighting by calling this method.

## See Also

### Related Documentation

class func unregisterClass(AnyClass)

Unregisters the specified subclass of URLProtocol.

class func registerClass(AnyClass) -> Bool

Attempts to register a subclass of URLProtocol, making it visible to the URL loading system.

URL Loading System

Interact with URLs and communicate with servers using standard Internet protocols.

