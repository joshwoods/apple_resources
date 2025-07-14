

- Foundation
- URL
-  fragment Deprecated

Instance Property

# fragment

The fragment component of the URL if the URL conforms to RFC 3986; otherwise, nil.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 8.0–18.4DeprecatedmacOS 10.10–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
var fragment: String? { get }
```

Deprecated

Use fragment(percentEncoded:) instead

## Discussion

Note

This function resolves against the base `URL`.

New code should use fragment(percentEncoded:) instead of this property.

## See Also

### Accessing the parts of a URL

func fragment(percentEncoded: Bool) -> String?

Returns the fragment component of the URL, optionally removing any percent-encoding.

func host(percentEncoded: Bool) -> String?

Returns the host component of the URL, optionally removing any percent-encoding.

var host: String?

The host component of a URL if the URL conforms to RFC 3986; otherwise, nil.

Deprecated

var lastPathComponent: String

The last path component of the URL, or an empty string if the path is an empty string.

func path(percentEncoded: Bool) -> String

Returns the path component of the URL, optionally removing any percent-encoding.

var path: String

The path component of the URL if the URL conforms to RFC 3986; otherwise, an empty string.

Deprecated

func password(percentEncoded: Bool) -> String?

Returns the password component of the URL, optionally removing any percent-encoding.

var password: String?

The password component of the URL if the URL conforms to RFC 3986; otherwise, nil.

Deprecated

var pathComponents: [String]

The path components of the URL, or an empty array if the path is an empty string.

var pathExtension: String

The path extension of the URL, or an empty string if the path is an empty string.

var port: Int?

The port component of the URL if the URL conforms to RFC 3986; otherwise, nil.

func query(percentEncoded: Bool) -> String?

Returns the query component of the URL, optionally removing any percent-encoding.

var query: String?

The query of the URL if the URL conforms to RFC 3986; otherwise, nil.

Deprecated

var scheme: String?

The scheme of the URL.

func user(percentEncoded: Bool) -> String?

Returns the user component of the URL, optionally removing any percent-encoding.

