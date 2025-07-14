

- Foundation
- URL
-  relativePath 

Instance Property

# relativePath

The relative path of the URL if the URL conforms to RFC 3986, otherwise nil.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var relativePath: String { get }
```

## Return Value

The relative path, or an empty string if the URL has an empty path.

## Discussion

Note

This function resolve against the base `URL`.

## See Also

### Accessing URL representations

var baseURL: URL?

The base URL.

var absoluteString: String

The absolute string for the URL.

var absoluteURL: URL

The absolute URL.

var relativeString: String

The relative portion of a URL.

var standardized: URL

A version of the URL with any instances of “..” or “.” resolved in its path.

var standardizedFileURL: URL

A standardized version of the path of a file URL.

