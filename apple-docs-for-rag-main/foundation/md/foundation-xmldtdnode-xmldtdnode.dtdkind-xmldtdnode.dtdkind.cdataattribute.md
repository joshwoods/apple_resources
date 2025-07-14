

- Foundation
- XMLDTDNode
- XMLDTDNode.DTDKind
-  XMLDTDNode.DTDKind.cdataAttribute 

Case

# XMLDTDNode.DTDKind.cdataAttribute

Identifies an attribute-list declaration with a `CDATA` (character data) value type.

Mac Catalyst 13.0+macOS 10.0+

``` source
case cdataAttribute
```

## See Also

### Enumeration Cases

case entitiesAttribute

Identifies an attribute-list declaration with an `ENTITIES` value type (refers to multiple unparsed entities declared elsewhere in document).

case entityAttribute

Identifies an attribute-list declaration with an `ENTITY` value type (refers to unparsed entity declared in document).

case enumerationAttribute

Identifies an attribute-list declaration with an enumeration value type (list of all possible values).

case idAttribute

Identifies an attribute-list declaration with an `ID` value type (per-document unique element name).

case idRefAttribute

Identifies an attribute-list declaration with an `IDREF` value type (refers to element `ID` type).

case idRefsAttribute

Identifies an attribute-list declaration with an `IDREFS` value type (refers to multiple elements of `ID` type).

case nmTokenAttribute

Identifies an attribute-list declaration with a `NMTOKEN` value type (name token).

case nmTokensAttribute

Identifies an attribute-list declaration with a `NMTOKENS` value type (multiple name tokens)

case notationAttribute

Identifies an attribute-list declaration with a `NOTATION` value type (name of declared notation).

case anyDeclaration

Identifies an `ANY` element declaration.

case elementDeclaration

Identifies a declaration of an element with child elements.

case emptyDeclaration

Identifies a declaration (`EMPTY`) of an empty element.

case mixedDeclaration

Identifies a declaration of an element with mixed content (`(#PCDATA | child)`).

case undefinedDeclaration

Identifies an undefined element declaration.

case general

Identifies a general entity declaration.

