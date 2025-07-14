

- Foundation
- XMLNode
-  localName(forName:) 

Type Method

# localName(forName:)

Returns the local name from the specified qualified name.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func localName(forName name: String) -> String
```

## Parameters 

`name`  

A string that is a qualified name.

## Discussion

For example, if the qualified name is “bst:title”, this method returns “title”.

## See Also

### Related Documentation

class func predefinedNamespace(forPrefix: String) -> XMLNode?

Returns an `NSXMLNode` object representing one of the predefined namespaces with the specified prefix.

### Managing Namespaces

var localName: String?

Returns the local name of the receiver.

var prefix: String?

Returns the prefix of the receiver’s name.

class func prefix(forName: String) -> String?

Returns the prefix from the specified qualified name.

