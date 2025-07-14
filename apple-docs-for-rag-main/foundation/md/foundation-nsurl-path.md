

- Foundation
- NSURL
-  path 

Instance Property

# path

The path, conforming to RFC 1808. (read-only)

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var path: String? { get }
```

## Discussion

This property contains the path, unescaped using the replacingPercentEscapes(using:) method. If the receiver does not conform to RFC 1808, this property contains `nil`.

If the receiver contains a file or file reference URL (as determined with isFileURL), this property’s value is suitable for input into methods of `NSFileManager` or `NSPathUtilities`. If the path has a trailing slash, it is stripped.

If the receiver contains a file reference URL, this property’s value provides the *current path* for the referenced resource, which may be `nil` if the resource no longer exists.

If the parameterString property contains a non-`nil` value, the path may be incomplete. If the receiver contains an unencoded semicolon, the path property ends at the character before the semicolon. The remainder of the URL is provided in the parameterString property.

To obtain the complete path, if parameterString contains a non-`nil` value, append a semicolon, followed by the parameter string.

Per RFC 3986, the leading slash after the authority (host name and port) portion is treated as part of the path. For example, in the URL `http://www.example.com/index.html`, the path is `/index.html`.

## See Also

### Accessing the Parts of the URL

var absoluteString: String?

The URL string for the receiver as an absolute URL. (read-only)

var absoluteURL: URL?

An absolute URL that refers to the same resource as the receiver. (read-only)

var baseURL: URL?

The base URL. (read-only)

var fileSystemRepresentation: UnsafePointer&lt;CChar>

A C string containing the URL’s file system path. (read-only)

var fragment: String?

The fragment identifier, conforming to RFC 1808. (read-only)

var host: String?

The host, conforming to RFC 1808. (read-only)

var lastPathComponent: String?

The last path component. (read-only)

var parameterString: String?

The parameter string conforming to RFC 1808. (read-only)

Deprecated

var password: String?

The password conforming to RFC 1808. (read-only)

var pathComponents: [String]?

An array containing the path components. (read-only)

var pathExtension: String?

The path extension. (read-only)

var port: NSNumber?

The port, conforming to RFC 1808.

var query: String?

The query string, conforming to RFC 1808.

var relativePath: String?

The relative path, conforming to RFC 1808. (read-only)

var relativeString: String

A string representation of the relative portion of the URL. (read-only)

