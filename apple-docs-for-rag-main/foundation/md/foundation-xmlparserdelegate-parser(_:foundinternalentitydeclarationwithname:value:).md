

- Foundation
- XMLParserDelegate
-  parser(\_:foundInternalEntityDeclarationWithName:value:) 

Instance Method

# parser(\_:foundInternalEntityDeclarationWithName:value:)

Sent by a parser object to the delegate when it encounters an internal entity declaration.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func parser(
    _ parser: XMLParser,
    foundInternalEntityDeclarationWithName name: String,
    value: String?
)
```

## Parameters 

`parser`  

An `NSXMLParser` object parsing XML.

`name`  

A string that is the declared name of an internal entity.

`value`  

A string that is the value of entity `name`.

## See Also

### Handling the DTD

func parser(XMLParser, foundAttributeDeclarationWithName: String, forElement: String, type: String?, defaultValue: String?)

Sent by a parser object to its delegate when it encounters a declaration of an attribute that is associated with a specific element.

func parser(XMLParser, foundElementDeclarationWithName: String, model: String)

Sent by a parser object to its delegate when it encounters a declaration of an element with a given model.

func parser(XMLParser, foundExternalEntityDeclarationWithName: String, publicID: String?, systemID: String?)

Sent by a parser object to its delegate when it encounters an external entity declaration.

func parser(XMLParser, foundUnparsedEntityDeclarationWithName: String, publicID: String?, systemID: String?, notationName: String?)

Sent by a parser object to its delegate when it encounters an unparsed entity declaration.

func parser(XMLParser, foundNotationDeclarationWithName: String, publicID: String?, systemID: String?)

Sent by a parser object to its delegate when it encounters a notation declaration.

