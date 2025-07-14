

- Foundation
- NSURLComponents
-  percentEncodedHost Deprecated

Instance Property

# percentEncodedHost

The host URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.9–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
var percentEncodedHost: String? { get set }
```

Deprecated

Use encodedHost instead

## Discussion

For example, in the URL `http://www.example.com/index.html`, the host is `www.example.com`.

If you set this value to something that is not a valid, percent-encoded string, this class throws an exception.

## See Also

### Accessing components in URL-encoded format

var percentEncodedFragment: String?

The fragment URL component (the part after a `#` symbol) expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedPassword: String?

The password URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedPath: String?

The path URL component expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedQuery: String?

The query URL component expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedUser: String?

The username URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

