

- Foundation
- URL
-  relativeString 

Instance Property

# relativeString

The relative portion of a URL.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var relativeString: String { get }
```

## Discussion

If `baseURL` is nil, or if the URL is itself absolute, this is the same as `absoluteString`.

## See Also

### Accessing URL representations

var baseURL: URL?

The base URL.

var absoluteString: String

The absolute string for the URL.

var absoluteURL: URL

The absolute URL.

var relativePath: String

The relative path of the URL if the URL conforms to RFC 3986, otherwise nil.

var standardized: URL

A version of the URL with any instances of “..” or “.” resolved in its path.

var standardizedFileURL: URL

A standardized version of the path of a file URL.

