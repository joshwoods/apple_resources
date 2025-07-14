

- Foundation
- NSURL
-  parameterString Deprecated

Instance Property

# parameterString

The parameter string conforming to RFC 1808. (read-only)

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
var parameterString: String? { get }
```

Deprecated

The parameterString method is deprecated. Post deprecation for applications linked with or after the macOS 10.15, and for all iOS, watchOS, and tvOS applications, parameterString will always return nil, and the path method will return the complete path including the semicolon separator and params component if the URL string contains them.

## Discussion

This property contains the parameter string. Any percent-encoded characters are not unescaped. If the receiver does not conform to RFC 1808, this property contains `nil`. For example, in the URL `file:///path/to/file;foo`, the parameter string is `foo`.

This property should not be confused with the query property, which also often contains a string of parameters.

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

var relativeString: String

A string representation of the relative portion of the URL. (read-only)

