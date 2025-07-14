

- Foundation
- NSURLComponents
-  percentEncodedUser 

Instance Property

# percentEncodedUser

The username URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var percentEncodedUser: String? { get set }
```

## Discussion

For example, in the URL `http://username:password@www.example.com/index.html`, the user is `username`.

If you set this value to something that is not a valid, percent-encoded string, this class throws an exception.

## See Also

### Accessing components in URL-encoded format

var percentEncodedFragment: String?

The fragment URL component (the part after a `#` symbol) expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedHost: String?

The host URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

Deprecated

var percentEncodedPassword: String?

The password URL subcomponent expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedPath: String?

The path URL component expressed as a URL-encoded string, or `nil` if not present.

var percentEncodedQuery: String?

The query URL component expressed as a URL-encoded string, or `nil` if not present.

