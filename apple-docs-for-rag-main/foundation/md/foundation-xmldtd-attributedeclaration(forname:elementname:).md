

- Foundation
- XMLDTD
-  attributeDeclaration(forName:elementName:) 

Instance Method

# attributeDeclaration(forName:elementName:)

Returns the DTD node representing an attribute-list declaration for a given attribute and its element.

Mac Catalyst 13.0+macOS 10.0+

``` source
func attributeDeclaration(
    forName name: String,
    elementName: String
) -> XMLDTDNode?
```

## Parameters 

`name`  

A string object identifying the name of an attribute.

`elementName`  

A string object identifying the name of an element.

## Return Value

An autoreleased XMLDTDNode object, or `nil` if there is no matching attribute-list declaration.

## Discussion

For example, in the attribute-list declaration:

```

```

“idnum” would correspond to `attrName` and “person” would correspond to `elementName`.

## See Also

### Getting DTD Nodes by Name

class func predefinedEntityDeclaration(forName: String) -> XMLDTDNode?

Returns a DTD node representing the predefined entity declaration with the specified name.

func elementDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing an element declaration for a specified element.

func entityDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing the entity declaration for a specified entity.

func notationDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing the notation declaration identified by the specified notation name.

