

- Foundation
- NSURL
-  resourceSpecifier 

Instance Property

# resourceSpecifier

The resource specifier. (read-only)

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var resourceSpecifier: String? { get }
```

## Discussion

This property contains the resource specifier. Any percent-encoded characters are not unescaped. For example, in the URL `http://www.example.com/index.html?key1=value1#jumplink`, the resource specifier is `//www.example.com/index.html?key1=value1#jumplink` (everything after the colon).

Important

If the receiver does not specify a net location portion of the URL, as returned by the toll-free bridged `CFURL` function CFURLCopyNetLocation(_:), then this method returns only the path of the receiver. For example, in the URL `file:///file.txt`, the resource specifier is `/file.txt`.

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

var path: String?

The path, conforming to RFC 1808. (read-only)

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

