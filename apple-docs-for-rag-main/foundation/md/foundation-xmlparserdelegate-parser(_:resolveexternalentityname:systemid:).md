

- Foundation
- XMLParserDelegate
-  parser(\_:resolveExternalEntityName:systemID:) 

Instance Method

# parser(\_:resolveExternalEntityName:systemID:)

Sent by a parser object to its delegate when it encounters a given external entity with a specific system ID.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func parser(
    _ parser: XMLParser,
    resolveExternalEntityName name: String,
    systemID: String?
) -> Data?
```

## Parameters 

`parser`  

A parser object.

`name`  

A string that specifies the external name of an entity.

`systemID`  

A string that specifies the system ID for the external entity.

## Return Value

An NSData object that contains the resolution of the given external entity.

## Discussion

The delegate can resolve the external entity (for example, locating and reading an externally declared DTD) and provide the result to the parser object as an `NSData` object.

## See Also

### Related Documentation

func parser(XMLParser, foundExternalEntityDeclarationWithName: String, publicID: String?, systemID: String?)

Sent by a parser object to its delegate when it encounters an external entity declaration.

func parser(XMLParser, foundUnparsedEntityDeclarationWithName: String, publicID: String?, systemID: String?, notationName: String?)

Sent by a parser object to its delegate when it encounters an unparsed entity declaration.

### Handling XML

func parserDidStartDocument(XMLParser)

Sent by the parser object to the delegate when it begins parsing a document.

func parserDidEndDocument(XMLParser)

Sent by the parser object to the delegate when it has successfully completed parsing.

func parser(XMLParser, didStartElement: String, namespaceURI: String?, qualifiedName: String?, attributes: [String : String])

Sent by a parser object to its delegate when it encounters a start tag for a given element.

func parser(XMLParser, didEndElement: String, namespaceURI: String?, qualifiedName: String?)

Sent by a parser object to its delegate when it encounters an end tag for a specific element.

func parser(XMLParser, didStartMappingPrefix: String, toURI: String)

Sent by a parser object to its delegate the first time it encounters a given namespace prefix, which is mapped to a URI.

func parser(XMLParser, didEndMappingPrefix: String)

Sent by a parser object to its delegate when a given namespace prefix goes out of scope.

func parser(XMLParser, parseErrorOccurred: any Error)

Sent by a parser object to its delegate when it encounters a fatal error.

func parser(XMLParser, validationErrorOccurred: any Error)

Sent by a parser object to its delegate when it encounters a fatal validation error. `NSXMLParser` currently does not invoke this method and does not perform validation.

func parser(XMLParser, foundCharacters: String)

Sent by a parser object to provide its delegate with a string representing all or part of the characters of the current element.

func parser(XMLParser, foundIgnorableWhitespace: String)

Reported by a parser object to provide its delegate with a string representing all or part of the ignorable whitespace characters of the current element.

func parser(XMLParser, foundProcessingInstructionWithTarget: String, data: String?)

Sent by a parser object to its delegate when it encounters a processing instruction.

func parser(XMLParser, foundComment: String)

Sent by a parser object to its delegate when it encounters a comment in the XML.

func parser(XMLParser, foundCDATA: Data)

Sent by a parser object to its delegate when it encounters a CDATA block.

