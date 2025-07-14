

- Foundation
- NSURLComponents
-  encodedHost 

Instance Property

# encodedHost

The host subcomponent, percent-encoded.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var encodedHost: String? { get set }
```

## Discussion

The getter for this property retains any percent-encoding this component may have. Setting this property assumes the component string already has the correct percent-encoding. Attempting to set an incorrectly percent-encoded string raises fatalError(_:file:line:).

## See Also

### Accessing components in native format

var fragment: String?

The fragment URL component (the part after a `#` symbol), or nil if not present.

var host: String?

The host URL subcomponent, or nil if not present.

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

