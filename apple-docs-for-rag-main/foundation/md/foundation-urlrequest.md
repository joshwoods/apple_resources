

- Foundation
-  URLRequest 

Structure

# URLRequest

A URL load request that is independent of protocol or URL scheme.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct URLRequest
```

## Mentioned in 

Uploading data to a website

Accessing cached data

Processing URL session data task results with Combine

Downloading files in the background

Downloading files from websites

## Overview

URLRequest encapsulates two essential properties of a load request: the URL to load and the policies used to load it. In addition, for HTTP and HTTPS requests, URLRequest includes the HTTP method (`GET`, `POST`, and so on) and the HTTP headers.

URLRequest only represents information about the request. Use other classes, such as URLSession, to send the request to a server. See Fetching website data into memory and Uploading data to a website for an introduction to these techniques.

When writing Swift code, favor this structure over the NSURLRequest and NSMutableURLRequest classes.

Certain header fields are reserved; see Reserved HTTP headers.

## Topics

### Creating a request

init(url: URL, cachePolicy: URLRequest.CachePolicy, timeoutInterval: TimeInterval)

Creates and initializes a URL request with the given URL, cache policy, and timeout interval.

### Working with a cache policy

var cachePolicy: URLRequest.CachePolicy

The request’s cache policy.

typealias CachePolicy

An alias for the cache policy.

enum CachePolicy

The constants used to specify interaction with the cached responses.

### Accessing request components

var httpMethod: String?

The HTTP request method.

var url: URL?

The URL of the request.

var httpBody: Data?

The data sent as the message body of a request, such as for an HTTP POST request.

var httpBodyStream: InputStream?

The stream used to deliver the HTTP body.

var mainDocumentURL: URL?

The main document URL associated with this request.

### Accessing header fields

var allHTTPHeaderFields: [String : String]?

A dictionary containing all of the HTTP header fields for a request.

func addValue(String, forHTTPHeaderField: String)

Adds a value to the header field.

func setValue(String?, forHTTPHeaderField: String)

Sets a value for the header field.

func value(forHTTPHeaderField: String) -> String?

Retrieves a header value.

### Controlling request behavior

var timeoutInterval: TimeInterval

The timeout interval of the request.

var httpShouldHandleCookies: Bool

A Boolean value indicating whether cookies will be sent with and set for this request.

var httpShouldUsePipelining: Bool

A Boolean value indicating whether the request should transmit before the previous response is received.

Deprecated

var allowsCellularAccess: Bool

A Boolean value indicating whether the request is allowed to use the built-in cellular radios to satisfy the request.

var allowsPersistentDNS: Bool

var assumesHTTP3Capable: Bool

var cookiePartitionIdentifier: String?

var requiresDNSSECValidation: Bool

### Supporting limited modes

var allowsConstrainedNetworkAccess: Bool

A Boolean value that indicates whether the request may use the network when the user has specified Low Data Mode.

var allowsExpensiveNetworkAccess: Bool

A Boolean value that indicates whether connections may use a network interface that the system considers expensive.

### Accessing the service type

var networkServiceType: URLRequest.NetworkServiceType

The type of network service for all tasks within network sessions to enable Cellular Network Slicing.

typealias NetworkServiceType

An alias for the network service type.

enum NetworkServiceType

Constants that specify how a request uses network resources.

### Indicating the source of the request

var attribution: URLRequest.Attribution

The entity that initiates the network request.

typealias Attribution

A type that indicates the entities that can make a network request.

### Using reference types

class NSURLRequest

A URL load request that is independent of protocol or URL scheme.

class NSMutableURLRequest

A mutable URL load request that is independent of protocol or URL scheme.

typealias MutableURLRequestDeprecated

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- ReferenceConvertible
- Sendable

## See Also

### Requests and responses

class NSURLRequest

A URL load request that is independent of protocol or URL scheme.

class NSMutableURLRequest

A mutable URL load request that is independent of protocol or URL scheme.

class URLResponse

The metadata associated with the response to a URL load request, independent of protocol and URL scheme.

class HTTPURLResponse

The metadata associated with the response to an HTTP protocol URL load request.

