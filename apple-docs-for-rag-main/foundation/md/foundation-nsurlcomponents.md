

- Foundation
-  NSURLComponents 

Class

# NSURLComponents

An object that parses URLs into and constructs URLs from their constituent parts.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSURLComponents
```

## Overview

In Swift, this object bridges to URLComponents; use NSURLComponents when you need reference semantics or other Foundation-specific behavior.

The NSURLComponents class is a class that is designed to parse URLs based on RFC 3986 and to construct URLs from their constituent parts. Its behavior differs subtly from the NSURL class, which conforms to older RFCs. However, you can easily obtain an NSURL object based on the contents of a URL components object or vice versa.

You create a URL components object in one of three ways: from an NSString object that contains a URL, from an NSURL object, or from scratch by using the default initializer. From there, you can modify the URL’s individual components and subcomponents by modifying various properties, either in unencoded form or in URL-encoded form. If you set the unencoded property, you can then obtain the encoded equivalent by reading the encoded property value and vice versa.

Important

The Swift overlay to the Foundation framework provides the URLComponents structure, which bridges to the NSURLComponents class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Creating URL components

init()

Creates a URL components object with all components left undefined.

init?(string: String)

Creates a URL components object by parsing a URL in string form.

init?(string: String, encodingInvalidCharacters: Bool)

Creates a URL components instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

init?(url: URL, resolvingAgainstBaseURL: Bool)

Creates a URL components object by parsing the URL from an `NSURL` object.

### Getting the URL

var string: String?

A URL derived from the components object, in string form.

var url: URL?

A URL object derived from the components object.

func url(relativeTo: URL?) -> URL?

Returns a URL object derived from the components object.

### Accessing components in native format

var fragment: String?

The fragment URL component (the part after a `#` symbol), or nil if not present.

var host: String?

The host URL subcomponent, or nil if not present.

var encodedHost: String?

The host subcomponent, percent-encoded.

var password: String?

The password URL subcomponent, or nil if not present.

var path: String?

The path URL component, or nil if not present.

var port: NSNumber?

The port number URL component, or nil if not present.

var query: String?

The query URL component as a string, or nil if not present.

var queryItems: [URLQueryItem]?

The query URL component as an array of name/value pairs.

var scheme: String?

The scheme URL component, or nil if not present.

var user: String?

The username URL subcomponent, or nil if not present.

### Accessing components in URL-encoded format

var percentEncodedFragment: String?

The fragment URL component (the part after a `#` symbol) expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedHost: String?

The host URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

Deprecated

var percentEncodedPassword: String?

The password URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedPath: String?

The path URL component expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedQuery: String?

The query URL component expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedUser: String?

The username URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

### Locating components in the URL string representation

var percentEncodedQueryItems: [URLQueryItem]?

var rangeOfFragment: NSRange

Returns the character range of the fragment in the string returned by the string property.

var rangeOfHost: NSRange

Returns the character range of the host in the string returned by the string property.

var rangeOfPassword: NSRange

Returns the character range of the password in the string returned by the string property.

var rangeOfPath: NSRange

Returns the character range of the path in the string returned by the string property.

var rangeOfPort: NSRange

Returns the character range of the port in the string returned by the string property.

var rangeOfQuery: NSRange

Returns the character range of the query in the string returned by the string property.

var rangeOfScheme: NSRange

Returns the character range of the scheme in the string returned by the string property.

var rangeOfUser: NSRange

Returns the character range of the user in the string returned by the string property.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

