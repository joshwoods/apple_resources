

- Foundation
- URLComponents
-  percentEncodedQueryItems 

Instance Property

# percentEncodedQueryItems

The query subcomponent, as an array of percent-encoded query items.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var percentEncodedQueryItems: [URLQueryItem]? { get set }
```

## Discussion

The setter combines an array containing any number of URLQueryItem key-value pairs into a query string and sets the `URLComponents` query property. This property assumes the query item names and values are already correctly percent-encoded. It also assumes that the query item names don’t contain the query item delimiter characters `&` and `=`. Attempting to set an incorrectly percent-encoded query item or a query item name with the query item delimiter characters `&` and `=` raises fatalError(_:file:line:).

## See Also

### Accessing components in URL-encoded format

var percentEncodedFragment: String?

The fragment subcomponent, percent-encoded.

var percentEncodedHost: String?

The host subcomponent, percent-encoded.

Deprecated

var percentEncodedPassword: String?

The password subcomponent, percent-encoded.

var percentEncodedPath: String

The path subcomponent, percent-encoded.

var percentEncodedQuery: String?

The query subcomponent, percent-encoded.

struct URLQueryItem

A single name-value pair from the query portion of a URL.

var percentEncodedUser: String?

The user subcomponent, percent-encoded.

