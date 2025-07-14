

- Foundation
- XMLParserDelegate
-  parser(\_:foundCDATA:) 

Instance Method

# parser(\_:foundCDATA:)

Sent by a parser object to its delegate when it encounters a CDATA block.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func parser(
    _ parser: XMLParser,
    foundCDATA CDATABlock: Data
)
```

## Parameters 

`parser`  

An `NSXMLParser` object parsing XML.

`CDATABlock`  

A data object containing a block of CDATA.

## Discussion

Through this method the parser object passes the contents of the block to its delegate in an NSData object. The CDATA block is character data that is ignored by the parser. The encoding of the character data is UTF-8. To convert the data object to a string object, use the `NSString` method init(data:encoding:).

## See Also

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

func parser(XMLParser, resolveExternalEntityName: String, systemID: String?) -> Data?

Sent by a parser object to its delegate when it encounters a given external entity with a specific system ID.

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

