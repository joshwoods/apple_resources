

- Foundation
- URLComponents
-  rangeOfUser 

Instance Property

# rangeOfUser

Returns the character range of the user in the string returned by the string property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var rangeOfUser: Range? { get }
```

## Discussion

If the component does not exist, nil is returned.

Note

Zero length components are legal. For example, the URL string “scheme://:@/?#” has a zero length user, password, host, query and fragment; the URL strings “scheme:” and “” both have a zero length path.

## See Also

### Locating components in the URL string representation

var rangeOfFragment: Range&lt;String.Index>?

Returns the character range of the fragment in the string returned by the string property.

var rangeOfHost: Range&lt;String.Index>?

Returns the character range of the host in the string returned by the string property.

var rangeOfPassword: Range&lt;String.Index>?

Returns the character range of the password in the string returned by the string property.

var rangeOfPath: Range&lt;String.Index>?

Returns the character range of the path in the string returned by the string property.

var rangeOfPort: Range&lt;String.Index>?

Returns the character range of the port in the string returned by the string property.

var rangeOfQuery: Range&lt;String.Index>?

Returns the character range of the query in the string returned by the string property.

var rangeOfScheme: Range&lt;String.Index>?

Returns the character range of the scheme in the string returned by the string property.

