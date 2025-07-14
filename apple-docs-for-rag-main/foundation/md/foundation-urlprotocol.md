

- Foundation
-  URLProtocol 

Class

# URLProtocol

An abstract class that handles the loading of protocol-specific URL data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLProtocol
```

## Overview

Don’t instantiate a URLProtocol subclass directly. Instead, create subclasses for any custom protocols or URL schemes that your app supports. When a download starts, the system creates the appropriate protocol object to handle the corresponding URL request. You define your protocol class and call the registerClass(_:) class method during your app’s launch time so that the system is aware of your protocol.

Note

You cannot use this class to define custom URL schemes and protocols in watchOS 2 and later.

To support the customization of protocol-specific requests, create extensions to the URLRequest class to provide any custom API that you need. You can store and retrieve protocol-specific request data by using URLProtocol’s class methods property(forKey:in:) and setProperty(_:forKey:in:).

Create a URLResponse for each request your subclass processes successfully. You may want to create a custom URLResponse class to provide protocol specific information.

### Subclassing notes

When overriding methods of this class, be aware that methods that take a `task` parameter are preferred by the system to those that do not. Therefore, you should override the task-based methods when subclassing, as follows:

Swift:

- Initialization — Override init(task:cachedResponse:client:) instead of or in addition to init(request:cachedResponse:client:). Also override the task-based canInit(with:) instead of or in addition to the request-based canInit(with:).

Objective-C:

- Initialization — Override canInit(with:) and init(task:cachedResponse:client:) instead of or in addition to canInit(with:) and init(request:cachedResponse:client:).

## Topics

### Creating protocol objects

init(request: URLRequest, cachedResponse: CachedURLResponse?, client: (any URLProtocolClient)?)

Creates a URL protocol instance to handle the request.

convenience init(task: URLSessionTask, cachedResponse: CachedURLResponse?, client: (any URLProtocolClient)?)

Creates a URL protocol instance to handle the task.

### Registering and unregistering protocol classes

class func registerClass(AnyClass) -> Bool

Attempts to register a subclass of URLProtocol, making it visible to the URL loading system.

class func unregisterClass(AnyClass)

Unregisters the specified subclass of URLProtocol.

### Determining If a subclass can handle a request

class func canInit(with: URLRequest) -> Bool

Determines whether the protocol subclass can handle the specified request.

class func canInit(with: URLSessionTask) -> Bool

Determines whether the protocol subclass can handle the specified task.

### Getting and setting request properties

class func property(forKey: String, in: URLRequest) -> Any?

Fetches the property associated with the specified key in the specified request.

class func setProperty(Any, forKey: String, in: NSMutableURLRequest)

Sets the property associated with the specified key in the specified request.

class func removeProperty(forKey: String, in: NSMutableURLRequest)

Removes the property associated with the specified key in the specified request.

### Providing a canonical version of a request

class func canonicalRequest(for: URLRequest) -> URLRequest

Returns a canonical version of the specified request.

### Determining if requests are cache equivalent

class func requestIsCacheEquivalent(URLRequest, to: URLRequest) -> Bool

A Boolean value indicating whether two requests are equivalent for cache purposes.

### Starting and stopping downloads

func startLoading()

Starts protocol-specific loading of the request.

func stopLoading()

Stops protocol-specific loading of the request.

### Getting protocol attributes

var cachedResponse: CachedURLResponse?

The protocol’s cached response.

var client: (any URLProtocolClient)?

The object the protocol uses to communicate with the URL loading system.

protocol URLProtocolClient

The interface used by URLProtocol subclasses to communicate with the URL Loading System.

var request: URLRequest

The protocol’s request.

var task: URLSessionTask?

The protocol’s task.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Supporting custom protocols

var protocolClasses: [AnyClass]?

An array of extra protocol subclasses that handle requests in a session.

