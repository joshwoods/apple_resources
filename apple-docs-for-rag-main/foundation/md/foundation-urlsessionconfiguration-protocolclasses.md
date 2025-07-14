

- Foundation
- URLSessionConfiguration
-  protocolClasses 

Instance Property

# protocolClasses

An array of extra protocol subclasses that handle requests in a session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var protocolClasses: [AnyClass]? { get set }
```

## Discussion

The objects in this array are `Class` objects corresponding to custom URLProtocol subclasses that you define. URL session objects support a number of common networking protocols by default. Use this array to extend the default set of common networking protocols available for use by a session with one or more custom protocols that you define.

Prior to handling a request, the URLSession object searches the default protocols first and then checks your custom protocols until it finds one capable of handling the specified request. It uses the protocol whose canInit(with:) class method returns true, indicating that the class is capable of handling the specified request.

Note

You cannot use custom URLProtocol subclasses in conjunction with background sessions.

The default value is an empty array.

## See Also

### Supporting custom protocols

class URLProtocol

An abstract class that handles the loading of protocol-specific URL data.

