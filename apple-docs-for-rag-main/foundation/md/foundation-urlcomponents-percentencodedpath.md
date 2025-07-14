

- Foundation
- URLComponents
-  percentEncodedPath 

Instance Property

# percentEncodedPath

The path subcomponent, percent-encoded.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var percentEncodedPath: String { get set }
```

## Discussion

The getter for this property retains any percent encoding this component may have. Setting this properties assumes the component string is already correctly percent encoded. Attempting to set an incorrectly percent encoded string will cause a `fatalError`. Although ‘;’ is a legal path character, it is recommended that it be percent-encoded for best compatibility with `URL` (`String.addingPercentEncoding(withAllowedCharacters:)` will percent-encode any ‘;’ characters if you pass `CharacterSet.urlPathAllowed`).

## See Also

### Accessing components in URL-encoded format

var percentEncodedFragment: String?

The fragment subcomponent, percent-encoded.

var percentEncodedHost: String?

The host subcomponent, percent-encoded.

Deprecated

var percentEncodedPassword: String?

The password subcomponent, percent-encoded.

var percentEncodedQuery: String?

The query subcomponent, percent-encoded.

var percentEncodedQueryItems: [URLQueryItem]?

The query subcomponent, as an array of percent-encoded query items.

struct URLQueryItem

A single name-value pair from the query portion of a URL.

var percentEncodedUser: String?

The user subcomponent, percent-encoded.

