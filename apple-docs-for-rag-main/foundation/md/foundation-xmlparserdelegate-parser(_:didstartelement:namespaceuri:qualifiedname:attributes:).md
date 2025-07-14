

- Foundation
- XMLParserDelegate
-  parser(\_:didStartElement:namespaceURI:qualifiedName:attributes:) 

Instance Method

# parser(\_:didStartElement:namespaceURI:qualifiedName:attributes:)

Sent by a parser object to its delegate when it encounters a start tag for a given element.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func parser(
    _ parser: XMLParser,
    didStartElement elementName: String,
    namespaceURI: String?,
    qualifiedName qName: String?,
    attributes attributeDict: [String : String] = [:]
)
```

## Parameters 

`parser`  

A parser object.

`elementName`  

A string that is the name of an element (in its start tag).

`namespaceURI`  

If namespace processing is turned on, contains the URI for the current namespace as a string object.

`qName`  

If namespace processing is turned on, contains the qualified name for the current namespace as a string object.

`attributeDict`  

A dictionary that contains any attributes associated with the element. Keys are the names of attributes, and values are attribute values.

## See Also

### Related Documentation

var shouldProcessNamespaces: Bool

A Boolean value that determines whether the parser reports the namespaces and qualified names of elements.

### Handling XML

func parserDidStartDocument(XMLParser)

Sent by the parser object to the delegate when it begins parsing a document.

func parserDidEndDocument(XMLParser)

Sent by the parser object to the delegate when it has successfully completed parsing.

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

func parser(XMLParser, foundCDATA: Data)

Sent by a parser object to its delegate when it encounters a CDATA block.

