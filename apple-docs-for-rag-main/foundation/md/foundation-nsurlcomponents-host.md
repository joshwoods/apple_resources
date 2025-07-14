

- Foundation
- NSURLComponents
-  host 

Instance Property

# host

The host URL subcomponent, or nil if not present.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var host: String? { get set }
```

## Discussion

For example, in the URL `http://www.example.com/index.html`, the host is `www.example.com`.

The getter for this property removes any percent encoding this component may have (if the component allows percent encoding). Setting this property assumes the subcomponent or component string isn’t percent encoded and adds percent encoding (if the component allows percent encoding).

## See Also

### Accessing components in native format

var fragment: String?

The fragment URL component (the part after a `#` symbol), or nil if not present.

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

