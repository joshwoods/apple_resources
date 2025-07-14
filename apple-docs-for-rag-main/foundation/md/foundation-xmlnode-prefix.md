

- Foundation
- XMLNode
-  prefix 

Instance Property

# prefix

Returns the prefix of the receiver’s name.

Mac Catalyst 13.0+macOS 10.0+

``` source
var prefix: String? { get }
```

## Return Value

A string containing the receiver’s prefix. This method returns an empty string if the receiver’s name is not qualified by a namespace.

## Discussion

The prefix is the part of a namespace-qualified name that precedes the colon. For example, “acme” is the prefix in the qualified name “acme:chapter”.

## See Also

### Managing Namespaces

var localName: String?

Returns the local name of the receiver.

class func localName(forName: String) -> String

Returns the local name from the specified qualified name.

class func prefix(forName: String) -> String?

Returns the prefix from the specified qualified name.

