

- Foundation
- XMLNode
-  prefix(forName:) 

Type Method

# prefix(forName:)

Returns the prefix from the specified qualified name.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func prefix(forName name: String) -> String?
```

## Parameters 

`name`  

A string that is a qualified name.

## Discussion

For example, if the qualified name is “bst:title”, this method returns “bst”.

## See Also

### Related Documentation

class func predefinedNamespace(forPrefix: String) -> XMLNode?

Returns an `NSXMLNode` object representing one of the predefined namespaces with the specified prefix.

### Managing Namespaces

var localName: String?

Returns the local name of the receiver.

class func localName(forName: String) -> String

Returns the local name from the specified qualified name.

var prefix: String?

Returns the prefix of the receiver’s name.

