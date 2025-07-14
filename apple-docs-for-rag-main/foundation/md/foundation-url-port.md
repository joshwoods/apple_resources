

- Foundation
- URL
-  port 

Instance Property

# port

The port component of the URL if the URL conforms to RFC 3986; otherwise, nil.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var port: Int? { get }
```

## Discussion

Note

This function resolves against the base `URL`.

## See Also

### Accessing the parts of a URL

func fragment(percentEncoded: Bool) -> String?

Returns the fragment component of the URL, optionally removing any percent-encoding.

var fragment: String?

The fragment component of the URL if the URL conforms to RFC 3986; otherwise, nil.

Deprecated

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

func query(percentEncoded: Bool) -> String?

Returns the query component of the URL, optionally removing any percent-encoding.

var query: String?

The query of the URL if the URL conforms to RFC 3986; otherwise, nil.

Deprecated

var scheme: String?

The scheme of the URL.

func user(percentEncoded: Bool) -> String?

Returns the user component of the URL, optionally removing any percent-encoding.

