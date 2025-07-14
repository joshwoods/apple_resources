

- Foundation
- XMLDTDNode
-  XMLDTDNode.DTDKind 

Enumeration

# XMLDTDNode.DTDKind

The type defined for the constants that specify the kind and subkind of DTD declaration represented by an `NSXMLDTDNode` object. You set the DTD-node kind using the doc:nsxmldtdnode/1806486-setdtdkind method.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum DTDKind
```

## Topics

### Enumeration Cases

case cdataAttribute

Identifies an attribute-list declaration with a `CDATA` (character data) value type.

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

case parameter

Identifies a parameter entity declaration.

case parsed

Identifies a parsed entity declaration.

case predefined

Identifies a predefined entity declaration.

case unparsed

Identifies an unparsed entity declaration.

case cdataAttribute

Identifies an attribute-list declaration with a `CDATA` (character data) value type.

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

case parameter

Identifies a parameter entity declaration.

case parsed

Identifies a parsed entity declaration.

case predefined

Identifies a predefined entity declaration.

case unparsed

Identifies an unparsed entity declaration.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

DTD Node Kind Constants

Constants that specify the kind and subkind of DTD declaration represented by an `NSXMLDTDNode` object. You set the DTD-node kind using the doc:nsxmldtdnode/1806486-setdtdkind method.

