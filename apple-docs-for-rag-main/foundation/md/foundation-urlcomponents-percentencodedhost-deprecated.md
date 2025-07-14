

- Foundation
- URLComponents
-  percentEncodedHost Deprecated

Instance Property

# percentEncodedHost

The host subcomponent, percent-encoded.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 8.0–18.4DeprecatedmacOS 10.10–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
var percentEncodedHost: String? { get set }
```

Deprecated

Use encodedHost instead.

## Discussion

The getter for this property retains any percent encoding this component may have. Setting this properties assumes the component string is already correctly percent encoded. Attempting to set an incorrectly percent encoded string will cause a `fatalError`. Although ‘;’ is a legal path character, it is recommended that it be percent-encoded for best compatibility with `URL` (`String.addingPercentEncoding(withAllowedCharacters:)` will percent-encode any ‘;’ characters if you pass `CharacterSet.urlHostAllowed`).

## See Also

### Accessing components in URL-encoded format

var percentEncodedFragment: String?

The fragment subcomponent, percent-encoded.

var percentEncodedPassword: String?

The password subcomponent, percent-encoded.

var percentEncodedPath: String

The path subcomponent, percent-encoded.

var percentEncodedQuery: String?

The query subcomponent, percent-encoded.

var percentEncodedQueryItems: [URLQueryItem]?

The query subcomponent, as an array of percent-encoded query items.

struct URLQueryItem

A single name-value pair from the query portion of a URL.

var percentEncodedUser: String?

The user subcomponent, percent-encoded.

