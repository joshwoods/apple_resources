

- Foundation
- NSURLComponents
-  scheme 

Instance Property

# scheme

The scheme URL component, or nil if not present.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var scheme: String? { get set }
```

## Discussion

For example, in the URL `http://www.example.com/index.html`, the scheme is `http`.

If you attempt to set the scheme to an invalid scheme string, this class throws an exception.

Note

The term “protocol” is also sometimes used when talking about network-based URL schemes. However, not all URL schemes are networking protocols—`data://` URLs, for example.

## See Also

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

var user: String?

The username URL subcomponent, or nil if not present.

