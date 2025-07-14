

- Core Foundation
- CFXMLNodeTypeCode
-  CFXMLNodeTypeCode.attributeListDeclaration 

Case

# CFXMLNodeTypeCode.attributeListDeclaration

Indicates an attribute list declaration where the data string is the tag name and the additional information is a pointer to a CFXMLAttributeListDeclarationInfo structure.

macOS

``` source
case attributeListDeclaration
```

## See Also

### Constants

case document

Indicates a document where the data string is `NULL` and the additional information is a pointer to a CFXMLDocumentInfo structure.

case element

Indicates an element where the data string is the name of the tag and the additional information is a pointer to a CFXMLElementInfo structure.

case attribute

Currently not used.

case processingInstruction

Indicates a processing instruction where the data string is the name of the target and the additional information is a pointer to a CFXMLProcessingInstructionInfo structure.

case comment

Indicates a comment section where the data string is the text of the comment and the additional information is `NULL`.

case text

Indicates a text section where the data string is the text’s contents and the additional information is `NULL`.

case cdataSection

Indicates a CDATA section where the data string is the text of the CDATA and the additional information is `NULL`.

case documentFragment

Currently not used.

case entity

Indicates an entity where the data string is the name of the entity and the additional information is a pointer to a CFXMLEntityInfo structure.

case entityReference

Indicates an entity reference where the data string is the name of the referenced entity and the additional information is a pointer to a CFXMLEntityReferenceInfo structure.

case documentType

Indicates a document type where the data string is the name given to the top-level element and the additional information is a pointer to a CFXMLDocumentTypeInfo structure.

case whitespace

Indicates white space where the data string is the text of the white space and the additional information is `NULL`.

case notation

Indicates a notation where the data string is the notation name and the additional information is a pointer to a CFXMLNotationInfo structure.

case elementTypeDeclaration

Indicates an element type declaration where the data string is the tag name and the additional information is a pointer to a CFXMLElementTypeDeclarationInfo structure.

