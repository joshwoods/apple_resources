

- Foundation
- XMLParserDelegate
-  parser(\_:foundElementDeclarationWithName:model:) 

Instance Method

# parser(\_:foundElementDeclarationWithName:model:)

Sent by a parser object to its delegate when it encounters a declaration of an element with a given model.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func parser(
    _ parser: XMLParser,
    foundElementDeclarationWithName elementName: String,
    model: String
)
```

## Parameters 

`parser`  

An `NSXMLParser` object parsing XML.

`elementName`  

A string that is the name of an element.

`model`  

A string that specifies a model for `elementName`.

## See Also

### Related Documentation

func parser(XMLParser, didStartElement: String, namespaceURI: String?, qualifiedName: String?, attributes: [String : String])

Sent by a parser object to its delegate when it encounters a start tag for a given element.

### Handling the DTD

func parser(XMLParser, foundAttributeDeclarationWithName: String, forElement: String, type: String?, defaultValue: String?)

Sent by a parser object to its delegate when it encounters a declaration of an attribute that is associated with a specific element.

func parser(XMLParser, foundExternalEntityDeclarationWithName: String, publicID: String?, systemID: String?)

Sent by a parser object to its delegate when it encounters an external entity declaration.

func parser(XMLParser, foundInternalEntityDeclarationWithName: String, value: String?)

Sent by a parser object to the delegate when it encounters an internal entity declaration.

func parser(XMLParser, foundUnparsedEntityDeclarationWithName: String, publicID: String?, systemID: String?, notationName: String?)

Sent by a parser object to its delegate when it encounters an unparsed entity declaration.

func parser(XMLParser, foundNotationDeclarationWithName: String, publicID: String?, systemID: String?)

Sent by a parser object to its delegate when it encounters a notation declaration.

