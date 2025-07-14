

- Foundation
- XMLParser
-  XMLParser.ErrorCode 

Enumeration

# XMLParser.ErrorCode

The following error codes are defined by `NSXMLParser`. For error codes not listed here, see the `` header file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum ErrorCode
```

## Topics

### Constants

case internalError

The parser object encountered an internal error.

case outOfMemoryError

The parser object ran out of memory.

case documentStartError

The parser object is unable to start parsing.

case emptyDocumentError

The document is empty.

case prematureDocumentEndError

The document ended unexpectedly.

case invalidHexCharacterRefError

Invalid hexadecimal character reference encountered.

case invalidDecimalCharacterRefError

Invalid decimal character reference encountered.

case invalidCharacterRefError

Invalid character reference encountered.

case invalidCharacterError

Invalid character encountered.

case characterRefAtEOFError

Target of character reference cannot be found.

case characterRefInPrologError

Invalid character found in the prolog.

case characterRefInEpilogError

Invalid character found in the epilog.

case characterRefInDTDError

Invalid character encountered in the DTD.

case entityRefAtEOFError

Target of entity reference is not found.

case entityRefInPrologError

Invalid entity reference found in the prolog.

case entityRefInEpilogError

Invalid entity reference found in the epilog.

case entityRefInDTDError

Invalid entity reference found in the DTD.

case parsedEntityRefAtEOFError

Target of parsed entity reference is not found.

case parsedEntityRefInPrologError

Target of parsed entity reference is not found in prolog.

case parsedEntityRefInEpilogError

Target of parsed entity reference is not found in epilog.

case parsedEntityRefInInternalSubsetError

Target of parsed entity reference is not found in internal subset.

case entityReferenceWithoutNameError

Entity reference is without name.

case entityReferenceMissingSemiError

Entity reference is missing semicolon.

case parsedEntityRefNoNameError

Parsed entity reference is without an entity name.

case parsedEntityRefMissingSemiError

Parsed entity reference is missing semicolon.

case undeclaredEntityError

Entity is not declared.

case unparsedEntityError

Cannot parse entity.

case entityIsExternalError

Cannot parse external entity.

case entityIsParameterError

Entity is a parameter.

case unknownEncodingError

Document encoding is unknown.

case encodingNotSupportedError

Document encoding is not supported.

case stringNotStartedError

String is not started.

case stringNotClosedError

String is not closed.

case namespaceDeclarationError

Invalid namespace declaration encountered.

case entityNotStartedError

Entity is not started.

case entityNotFinishedError

Entity is not finished.

case lessThanSymbolInAttributeError

Angle bracket is used in attribute.

case attributeNotStartedError

Attribute is not started.

case attributeNotFinishedError

Attribute is not finished.

case attributeHasNoValueError

Attribute doesn’t contain a value.

case attributeRedefinedError

Attribute is redefined.

case literalNotStartedError

Literal is not started.

case literalNotFinishedError

Literal is not finished.

case commentNotFinishedError

Comment is not finished.

case processingInstructionNotStartedError

Processing instruction is not started.

case processingInstructionNotFinishedError

Processing instruction is not finished.

case notationNotStartedError

Notation is not started.

case notationNotFinishedError

Notation is not finished.

case attributeListNotStartedError

Attribute list is not started.

case attributeListNotFinishedError

Attribute list is not finished.

case mixedContentDeclNotStartedError

Mixed content declaration is not started.

case mixedContentDeclNotFinishedError

Mixed content declaration is not finished.

case elementContentDeclNotStartedError

Element content declaration is not started.

case elementContentDeclNotFinishedError

Element content declaration is not finished.

case xmlDeclNotStartedError

XML declaration is not started.

case xmlDeclNotFinishedError

XML declaration is not finished.

case conditionalSectionNotStartedError

Conditional section is not started.

case conditionalSectionNotFinishedError

Conditional section is not finished.

case externalSubsetNotFinishedError

External subset is not finished.

case doctypeDeclNotFinishedError

Document type declaration is not finished.

case misplacedCDATAEndStringError

Misplaced CDATA end string.

case cdataNotFinishedError

CDATA block is not finished.

case misplacedXMLDeclarationError

Misplaced XML declaration.

case spaceRequiredError

Space is required.

case separatorRequiredError

Separator is required.

case nmtokenRequiredError

Name token is required.

case nameRequiredError

Name is required.

case pcdataRequiredError

CDATA is required.

case uriRequiredError

URI is required.

case publicIdentifierRequiredError

Public identifier is required.

case ltRequiredError

Left angle bracket is required.

case gtRequiredError

Right angle bracket is required.

case ltSlashRequiredError

Left angle bracket slash is required.

case equalExpectedError

Equal sign expected.

case tagNameMismatchError

Tag name mismatch.

case unfinishedTagError

Unfinished tag found.

case standaloneValueError

Standalone value found.

case invalidEncodingNameError

Invalid encoding name found.

case commentContainsDoubleHyphenError

Comment contains double hyphen.

case invalidEncodingError

Invalid encoding.

case externalStandaloneEntityError

External standalone entity.

case invalidConditionalSectionError

Invalid conditional section.

case entityValueRequiredError

Entity value is required.

case notWellBalancedError

Document is not well balanced.

case extraContentError

Error in content found.

case invalidCharacterInEntityError

Invalid character in entity found.

case parsedEntityRefInInternalError

Internal error in parsed entity reference found.

case entityRefLoopError

Entity reference loop encountered.

case entityBoundaryError

Entity boundary error.

case invalidURIError

Invalid URI specified.

case uriFragmentError

URI fragment.

case noDTDError

Missing DTD.

case delegateAbortedParseError

Delegate aborted parse.

case internalError

The parser object encountered an internal error.

case outOfMemoryError

The parser object ran out of memory.

case documentStartError

The parser object is unable to start parsing.

case emptyDocumentError

The document is empty.

case prematureDocumentEndError

The document ended unexpectedly.

case invalidHexCharacterRefError

Invalid hexadecimal character reference encountered.

case invalidDecimalCharacterRefError

Invalid decimal character reference encountered.

case invalidCharacterRefError

Invalid character reference encountered.

case invalidCharacterError

Invalid character encountered.

case characterRefAtEOFError

Target of character reference cannot be found.

case characterRefInPrologError

Invalid character found in the prolog.

case characterRefInEpilogError

Invalid character found in the epilog.

case characterRefInDTDError

Invalid character encountered in the DTD.

case entityRefAtEOFError

Target of entity reference is not found.

case entityRefInPrologError

Invalid entity reference found in the prolog.

case entityRefInEpilogError

Invalid entity reference found in the epilog.

case entityRefInDTDError

Invalid entity reference found in the DTD.

case parsedEntityRefAtEOFError

Target of parsed entity reference is not found.

case parsedEntityRefInPrologError

Target of parsed entity reference is not found in prolog.

case parsedEntityRefInEpilogError

Target of parsed entity reference is not found in epilog.

case parsedEntityRefInInternalSubsetError

Target of parsed entity reference is not found in internal subset.

case entityReferenceWithoutNameError

Entity reference is without name.

case entityReferenceMissingSemiError

Entity reference is missing semicolon.

case parsedEntityRefNoNameError

Parsed entity reference is without an entity name.

case parsedEntityRefMissingSemiError

Parsed entity reference is missing semicolon.

case undeclaredEntityError

Entity is not declared.

case unparsedEntityError

Cannot parse entity.

case entityIsExternalError

Cannot parse external entity.

case entityIsParameterError

Entity is a parameter.

case unknownEncodingError

Document encoding is unknown.

case encodingNotSupportedError

Document encoding is not supported.

case stringNotStartedError

String is not started.

case stringNotClosedError

String is not closed.

case namespaceDeclarationError

Invalid namespace declaration encountered.

case entityNotStartedError

Entity is not started.

case entityNotFinishedError

Entity is not finished.

case lessThanSymbolInAttributeError

Angle bracket is used in attribute.

case attributeNotStartedError

Attribute is not started.

case attributeNotFinishedError

Attribute is not finished.

case attributeHasNoValueError

Attribute doesn’t contain a value.

case attributeRedefinedError

Attribute is redefined.

case literalNotStartedError

Literal is not started.

case literalNotFinishedError

Literal is not finished.

case commentNotFinishedError

Comment is not finished.

case processingInstructionNotStartedError

Processing instruction is not started.

case processingInstructionNotFinishedError

Processing instruction is not finished.

case notationNotStartedError

Notation is not started.

case notationNotFinishedError

Notation is not finished.

case attributeListNotStartedError

Attribute list is not started.

case attributeListNotFinishedError

Attribute list is not finished.

case mixedContentDeclNotStartedError

Mixed content declaration is not started.

case mixedContentDeclNotFinishedError

Mixed content declaration is not finished.

case elementContentDeclNotStartedError

Element content declaration is not started.

case elementContentDeclNotFinishedError

Element content declaration is not finished.

case xmlDeclNotStartedError

XML declaration is not started.

case xmlDeclNotFinishedError

XML declaration is not finished.

case conditionalSectionNotStartedError

Conditional section is not started.

case conditionalSectionNotFinishedError

Conditional section is not finished.

case externalSubsetNotFinishedError

External subset is not finished.

case doctypeDeclNotFinishedError

Document type declaration is not finished.

case misplacedCDATAEndStringError

Misplaced CDATA end string.

case cdataNotFinishedError

CDATA block is not finished.

case misplacedXMLDeclarationError

Misplaced XML declaration.

case spaceRequiredError

Space is required.

case separatorRequiredError

Separator is required.

case nmtokenRequiredError

Name token is required.

case nameRequiredError

Name is required.

case pcdataRequiredError

CDATA is required.

case uriRequiredError

URI is required.

case publicIdentifierRequiredError

Public identifier is required.

case ltRequiredError

Left angle bracket is required.

case gtRequiredError

Right angle bracket is required.

case ltSlashRequiredError

Left angle bracket slash is required.

case equalExpectedError

Equal sign expected.

case tagNameMismatchError

Tag name mismatch.

case unfinishedTagError

Unfinished tag found.

case standaloneValueError

Standalone value found.

case invalidEncodingNameError

Invalid encoding name found.

case commentContainsDoubleHyphenError

Comment contains double hyphen.

case invalidEncodingError

Invalid encoding.

case externalStandaloneEntityError

External standalone entity.

case invalidConditionalSectionError

Invalid conditional section.

case entityValueRequiredError

Entity value is required.

case notWellBalancedError

Document is not well balanced.

case extraContentError

Error in content found.

case invalidCharacterInEntityError

Invalid character in entity found.

case parsedEntityRefInInternalError

Internal error in parsed entity reference found.

case entityRefLoopError

Entity reference loop encountered.

case entityBoundaryError

Entity boundary error.

case invalidURIError

Invalid URI specified.

case uriFragmentError

URI fragment.

case noDTDError

Missing DTD.

case delegateAbortedParseError

Delegate aborted parse.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum ExternalEntityResolvingPolicy

class let errorDomain: String

Indicates an error in XML parsing.

