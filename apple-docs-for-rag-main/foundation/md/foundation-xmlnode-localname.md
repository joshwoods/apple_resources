

- Foundation
- XMLNode
-  localName 

Instance Property

# localName

Returns the local name of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var localName: String? { get }
```

## Return Value

A string containing the local name of the receiver.

## Discussion

The local name is the part of a node name that follows a namespace-qualifying colon or the full name if there is no colon. For example, “chapter” is the local name in the qualified name “acme:chapter”.

## See Also

### Managing Namespaces

class func localName(forName: String) -> String

Returns the local name from the specified qualified name.

var prefix: String?

Returns the prefix of the receiver’s name.

class func prefix(forName: String) -> String?

Returns the prefix from the specified qualified name.

