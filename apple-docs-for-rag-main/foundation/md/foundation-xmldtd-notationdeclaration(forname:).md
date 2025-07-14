

- Foundation
- XMLDTD
-  notationDeclaration(forName:) 

Instance Method

# notationDeclaration(forName:)

Returns the DTD node representing the notation declaration identified by the specified notation name.

Mac Catalyst 13.0+macOS 10.0+

``` source
func notationDeclaration(forName name: String) -> XMLDTDNode?
```

## Parameters 

`name`  

A string that is the name of a notation.

## Return Value

An autoreleased XMLDTDNode object, or `nil` if there is no match.

## See Also

### Getting DTD Nodes by Name

class func predefinedEntityDeclaration(forName: String) -> XMLDTDNode?

Returns a DTD node representing the predefined entity declaration with the specified name.

func elementDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing an element declaration for a specified element.

func attributeDeclaration(forName: String, elementName: String) -> XMLDTDNode?

Returns the DTD node representing an attribute-list declaration for a given attribute and its element.

func entityDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing the entity declaration for a specified entity.

