

- Foundation
- URLSession
-  configuration 

Instance Property

# configuration

A copy of the configuration object for this session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var configuration: URLSessionConfiguration { get }
```

## Mentioned in 

Accessing cached data

## Discussion

Beginning in iOS 9 and OS X 10.11, URLSession objects store a copy of the URLSessionConfiguration object passed to their initializers, such that a session’s configuration is immutable after initialization. Any further changes to mutable properties on the configuration object passed to a session’s initializer or the value returned from a session’s configuration property do not affect the behavior of that session. However, you can create a new session with the modified configuration object.

Note

On previous versions of iOS and macOS, a bug in the implementation causes URLSession objects to store a *reference* to configuration objects passed to their initializers rather than a copy. This allows the behavior of a session to be further configured after initialization by modifying the configuration object passed to a session’s initializer or the value returned from a session’s configuration property. You can ensure consistent behavior across different platform versions by explicitly calling copy() on configuration objects passed to a URLSession initializer or returned from the configuration property.

## See Also

### Creating a session

init(configuration: URLSessionConfiguration)

Creates a session with the specified session configuration.

init(configuration: URLSessionConfiguration, delegate: (any URLSessionDelegate)?, delegateQueue: OperationQueue?)

Creates a session with the specified session configuration, delegate, and operation queue.

class URLSessionConfiguration

A configuration object that defines behavior and policies for a URL session.

