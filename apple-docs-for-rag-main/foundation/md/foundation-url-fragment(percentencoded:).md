

- Foundation
- URL
-  fragment(percentEncoded:) 

Instance Method

# fragment(percentEncoded:)

Returns the fragment component of the URL, optionally removing any percent-encoding.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func fragment(percentEncoded: Bool = true) -> String?
```

## Parameters 

`percentEncoded`  

A Boolean value that indicates whether the URL percent-encodes any unreserved characters. Defaults to `true`.

## Return Value

The fragment component of the URL, optionally percent-encoding any unreserved characters.

## Discussion

The system doesn’t allow certain characters in the URL fragment component, so URL percent-encodes those characters to create a valid URL. Calling this function with `percentEncoded = false` removes any percent-encoding and returns the unencoded fragment.

If the URL doesn’t contain a fragment component according to RFC 3986, this function returns `nil`.

## See Also

### Accessing the parts of a URL

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

