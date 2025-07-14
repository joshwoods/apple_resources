

- Foundation
- XMLDTD
-  predefinedEntityDeclaration(forName:) 

Type Method

# predefinedEntityDeclaration(forName:)

Returns a DTD node representing the predefined entity declaration with the specified name.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func predefinedEntityDeclaration(forName name: String) -> XMLDTDNode?
```

## Parameters 

`name`  

A string identifying a predefined entity declaration.

## Return Value

An autoreleased XMLDTDNode object, or `nil` if there is no match for `name`.

## Discussion

The five predefined entity references (or character references) are “\” (greater-than sign), “&” (ampersand), “"” (quotation mark), and “'” (apostrophe).

## See Also

### Getting DTD Nodes by Name

func elementDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing an element declaration for a specified element.

func attributeDeclaration(forName: String, elementName: String) -> XMLDTDNode?

Returns the DTD node representing an attribute-list declaration for a given attribute and its element.

func entityDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing the entity declaration for a specified entity.

func notationDeclaration(forName: String) -> XMLDTDNode?

Returns the DTD node representing the notation declaration identified by the specified notation name.

