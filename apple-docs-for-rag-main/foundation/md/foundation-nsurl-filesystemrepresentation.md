

- Foundation
- NSURL
-  fileSystemRepresentation 

Instance Property

# fileSystemRepresentation

A C string containing the URL’s file system path. (read-only)

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var fileSystemRepresentation: UnsafePointer { get }
```

## Discussion

This returns a null-terminated C string in file system representation.

This string is automatically freed in the same way that a returned object would be released. The caller must either copy the string or use getFileSystemRepresentation(_:maxLength:) if it needs to store the representation outside of the autorelease context in which the value was obtained.

The file system representation format is described in File Encodings and Fonts.

## See Also

### Accessing the Parts of the URL

var absoluteString: String?

The URL string for the receiver as an absolute URL. (read-only)

var absoluteURL: URL?

An absolute URL that refers to the same resource as the receiver. (read-only)

var baseURL: URL?

The base URL. (read-only)

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

var relativeString: String

A string representation of the relative portion of the URL. (read-only)

