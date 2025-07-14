

- Foundation
- NSURLComponents
-  percentEncodedPath 

Instance Property

# percentEncodedPath

The path URL component expressed as a URL-encoded string, or `nil` if not present.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var percentEncodedPath: String? { get set }
```

## Discussion

For example, in the URL `http://www.example.com/index.html`, the path is `/index.html`.

If you set this value to something that is not a valid, percent-encoded string, this class throws an exception.

Note

Although an unencoded semicolon is a valid character in a percent-encoded path, for compatibility with the NSURL class, you should always percent-encode it. To properly encode a string for use in the path component of a URL, use the character set returned by the `URLPathAllowedCharacterSet` method in conjunction with the addingPercentEncoding(withAllowedCharacters:) method.

## See Also

### Accessing components in URL-encoded format

var percentEncodedFragment: String?

The fragment URL component (the part after a `#` symbol) expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedHost: String?

The host URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

Deprecated

var percentEncodedPassword: String?

The password URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedQuery: String?

The query URL component expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedUser: String?

The username URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

