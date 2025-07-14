

- Foundation
- URLComponents
-  queryItems 

Instance Property

# queryItems

An array of query items for the URL in the order in which they appear in the original query string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var queryItems: [URLQueryItem]? { get set }
```

## Discussion

Each `URLQueryItem` represents a single key-value pair,

Note that a name may appear more than once in a single query string, so the name values are not guaranteed to be unique. If the `URLComponents` has an empty query component, returns an empty array. If the `URLComponents` has no query component, returns nil.

The setter combines an array containing any number of `URLQueryItem`s, each of which represents a single key-value pair, into a query string and sets the `URLComponents` query property. Passing an empty array sets the query component of the `URLComponents` to an empty string. Passing nil removes the query component of the `URLComponents`.

Note

If a name-value pair in a query is empty (i.e. the query string starts with ‘&’, ends with ‘&’, or has “&&” within it), you get a `URLQueryItem` with a zero-length name and a nil value. If a query’s name-value pair has nothing before the equals sign, you get a zero-length name. If a query’s name-value pair has nothing after the equals sign, you get a zero-length value. If a query’s name-value pair has no equals sign, the query name-value pair string is the name and you get a nil value.

## See Also

### Accessing components in native format

var fragment: String?

The fragment subcomponent.

var host: String?

The host subcomponent.

var encodedHost: String?

The host subcomponent, percent-encoded.

var password: String?

The password subcomponent of the URL.

var path: String

The path subcomponent.

var port: Int?

The port subcomponent.

var query: String?

The query subcomponent.

var scheme: String?

The scheme subcomponent of the URL.

var user: String?

The user subcomponent of the URL.

