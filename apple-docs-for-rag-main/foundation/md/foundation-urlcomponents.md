

- Foundation
-  URLComponents 

Structure

# URLComponents

A structure that parses URLs into and constructs URLs from their constituent parts.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct URLComponents
```

## Overview

This structure parses and constructs URLs according to RFC 3986. Its behavior differs subtly from that of the URL structure, which conforms to older RFCs. However, you can easily obtain a URL value based on the contents of a URLComponents value or vice versa.

## Topics

### Creating URL components

init()

Creates a URL components instance without defining any of the components.

init?(string: String)

Creates a URL components instance from a URL string.

init?(string: String, encodingInvalidCharacters: Bool)

Creates a URL components instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

init?(url: URL, resolvingAgainstBaseURL: Bool)

Creates a URL components instance from a URL string, optionally resolving against a base URL.

### Getting the URL

var url: URL?

A URL created from the components.

func url(relativeTo: URL?) -> URL?

Returns a URL based on the component settings and relative to a given base URL.

var string: String?

A URL derived from the components object, in string form.

### Accessing components in native format

var fragment: String?

The fragment subcomponent.

var host: String?

The host subcomponent.

var encodedHost: String?

The host subcomponent, percent-encoded.

var password: String?

The password subcomponent of the URL.

var path: String

The path subcomponent.

var port: Int?

The port subcomponent.

var query: String?

The query subcomponent.

var queryItems: [URLQueryItem]?

An array of query items for the URL in the order in which they appear in the original query string.

var scheme: String?

The scheme subcomponent of the URL.

var user: String?

The user subcomponent of the URL.

### Accessing components in URL-encoded format

var percentEncodedFragment: String?

The fragment subcomponent, percent-encoded.

var percentEncodedHost: String?

The host subcomponent, percent-encoded.

Deprecated

var percentEncodedPassword: String?

The password subcomponent, percent-encoded.

var percentEncodedPath: String

The path subcomponent, percent-encoded.

var percentEncodedQuery: String?

The query subcomponent, percent-encoded.

var percentEncodedQueryItems: [URLQueryItem]?

The query subcomponent, as an array of percent-encoded query items.

struct URLQueryItem

A single name-value pair from the query portion of a URL.

var percentEncodedUser: String?

The user subcomponent, percent-encoded.

### Locating components in the URL string representation

var rangeOfFragment: Range&lt;String.Index>?

Returns the character range of the fragment in the string returned by the string property.

var rangeOfHost: Range&lt;String.Index>?

Returns the character range of the host in the string returned by the string property.

var rangeOfPassword: Range&lt;String.Index>?

Returns the character range of the password in the string returned by the string property.

var rangeOfPath: Range&lt;String.Index>?

Returns the character range of the path in the string returned by the string property.

var rangeOfPort: Range&lt;String.Index>?

Returns the character range of the port in the string returned by the string property.

var rangeOfQuery: Range&lt;String.Index>?

Returns the character range of the query in the string returned by the string property.

var rangeOfScheme: Range&lt;String.Index>?

Returns the character range of the scheme in the string returned by the string property.

var rangeOfUser: Range&lt;String.Index>?

Returns the character range of the user in the string returned by the string property.

### Using reference types

class NSURLComponents

An object that parses URLs into and constructs URLs from their constituent parts.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- ReferenceConvertible
- Sendable

## See Also

### URLs

struct URL

A value that identifies the location of a resource, such as an item on a remote server or the path to a local file.

struct URLQueryItem

A single name-value pair from the query portion of a URL.

