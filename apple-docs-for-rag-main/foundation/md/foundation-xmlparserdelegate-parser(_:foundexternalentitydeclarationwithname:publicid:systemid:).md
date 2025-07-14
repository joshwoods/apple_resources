

- Foundation
- XMLParserDelegate
-  parser(\_:foundExternalEntityDeclarationWithName:publicID:systemID:) 

Instance Method

# parser(\_:foundExternalEntityDeclarationWithName:publicID:systemID:)

Sent by a parser object to its delegate when it encounters an external entity declaration.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func parser(
    _ parser: XMLParser,
    foundExternalEntityDeclarationWithName name: String,
    publicID: String?,
    systemID: String?
)
```

## Parameters 

`parser`  

An `NSXMLParser` object parsing XML.

`name`  

A string that is the name of an entity.

`publicID`  

A string that specifies the public ID associated with `entityName`.

`systemID`  

A string that specifies the system ID associated with `entityName`.

## See Also

### Related Documentation

func parser(XMLParser, resolveExternalEntityName: String, systemID: String?) -> Data?

Sent by a parser object to its delegate when it encounters a given external entity with a specific system ID.

### Handling the DTD

func parser(XMLParser, foundAttributeDeclarationWithName: String, forElement: String, type: String?, defaultValue: String?)

Sent by a parser object to its delegate when it encounters a declaration of an attribute that is associated with a specific element.

func parser(XMLParser, foundElementDeclarationWithName: String, model: String)

Sent by a parser object to its delegate when it encounters a declaration of an element with a given model.

func parser(XMLParser, foundInternalEntityDeclarationWithName: String, value: String?)

Sent by a parser object to the delegate when it encounters an internal entity declaration.

func parser(XMLParser, foundUnparsedEntityDeclarationWithName: String, publicID: String?, systemID: String?, notationName: String?)

Sent by a parser object to its delegate when it encounters an unparsed entity declaration.

func parser(XMLParser, foundNotationDeclarationWithName: String, publicID: String?, systemID: String?)

Sent by a parser object to its delegate when it encounters a notation declaration.

