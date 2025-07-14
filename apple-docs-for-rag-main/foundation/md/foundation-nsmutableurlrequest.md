

- Foundation
-  NSMutableURLRequest 

Class

# NSMutableURLRequest

A mutable URL load request that is independent of protocol or URL scheme.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMutableURLRequest
```

## Overview

In Swift, this object bridges to NSURLRequest and you use when you need reference semantics or other Foundation-specific behavior.

NSMutableURLRequest is a subclass of NSURLRequest that allows you to change the request’s properties.

NSMutableURLRequest only represents information about the request. Use other classes, such as URLSession, to send the request to a server. See Fetching website data into memory and Uploading data to a website for an introduction to these techniques.

Classes that create a network operation based on a request make a deep copy of that request. Thus, changing the request after creating a network operation has no effect on the ongoing operation. For example, if you use dataTask(with:completionHandler:) to create a data task from a request, and then later change the request, the data task continues using the original request.

Important

The Swift overlay to the Foundation framework provides the URLRequest structure, which bridges to the NSMutableURLRequest class and its immutable superclass, NSURLRequest. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Working with a cache policy

var cachePolicy: NSURLRequest.CachePolicy

The request’s cache policy.

enum CachePolicy

The constants used to specify interaction with the cached responses.

### Accessing request components

var httpMethod: String

The HTTP request method.

var url: URL?

The URL being requested.

var httpBody: Data?

The request body.

var httpBodyStream: InputStream?

The request body as an input stream.

var mainDocumentURL: URL?

The main document URL.

### Accessing header fields

var allHTTPHeaderFields: [String : String]?

A dictionary containing all of the HTTP header fields for a request.

func addValue(String, forHTTPHeaderField: String)

Adds a value to the header field.

func setValue(String?, forHTTPHeaderField: String)

Sets a value for the header field.

### Controlling request behavior

var timeoutInterval: TimeInterval

The request’s timeout interval, in seconds.

var httpShouldHandleCookies: Bool

A Boolean value that indicates whether the request should use the default cookie handling for the request.

var httpShouldUsePipelining: Bool

A Boolean value that indicates whether the request can continue transmitting data before receiving a response from an earlier transmission.

Deprecated

var allowsCellularAccess: Bool

A Boolean value that indicates whether a connection can use the device’s cellular network (if present).

### Supporting limited modes

var allowsConstrainedNetworkAccess: Bool

A Boolean value that indicates whether connections may use the network when the user has specified Low Data Mode.

var allowsExpensiveNetworkAccess: Bool

A Boolean value that indicates whether connections may use a network interface that the system considers expensive.

### Accessing the service type

var networkServiceType: NSURLRequest.NetworkServiceType

The network service type of the connection.

enum NetworkServiceType

Constants that specify how a request uses network resources.

### Working with hotspots

func bind(to: NEHotspotHelperCommand)

Binds a URL request to the network interface associated with the hotspot helper command instance.

### Indicating the source of the request

var attribution: NSURLRequest.Attribution

The entity that initiates the network request.

enum Attribution

The entities that can make a network request.

### Instance Properties

var allowsPersistentDNS: Bool

var assumesHTTP3Capable: Bool

var cookiePartitionIdentifier: String?

var requiresDNSSECValidation: Bool

## Relationships

### Inherits From

- NSURLRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Requests and responses

struct URLRequest

A URL load request that is independent of protocol or URL scheme.

class NSURLRequest

A URL load request that is independent of protocol or URL scheme.

class URLResponse

The metadata associated with the response to a URL load request, independent of protocol and URL scheme.

class HTTPURLResponse

The metadata associated with the response to an HTTP protocol URL load request.

