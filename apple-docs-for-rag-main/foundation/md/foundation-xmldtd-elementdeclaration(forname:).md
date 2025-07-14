

- Foundation
- XMLDTD
-  elementDeclaration(forName:) 

Instance Method

# elementDeclaration(forName:)

Returns the DTD node representing an element declaration for a specified element.

Mac Catalyst 13.0+macOS 10.0+

``` source
func elementDeclaration(forName name: String) -> XMLDTDNode?
```

## Parameters 

`name`  

A string that is the name of an element.

## Return Value

An autoreleased XMLDTDNode object, or `nil` if there is no match.

## See Also

### Getting DTD Nodes by Name

class func predefinedEntityDeclaration(forName: String) -> XMLDTDNode?

Returns a DTD node representing the predefined entity declaration with the specified name.

func attributeDeclaration(forName: String, elementName: String) -> XMLDTDNode?

Returns the DTD node representing an attribute-list declaration for a given attribute and its element.

func entityDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing the entity declaration for a specified entity.

func notationDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing the notation declaration identified by the specified notation name.

