

- Foundation
-  XMLParser 

Class

# XMLParser

An event driven parser of XML documents (including DTD declarations).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class XMLParser
```

## Overview

An XMLParser notifies its delegate about the items (elements, attributes, CDATA blocks, comments, and so on) that it encounters as it processes an XML document. It does not itself do anything with those parsed items except report them. It also reports parsing errors. For convenience, an XMLParser object in the following descriptions is sometimes referred to as a parser object. Unless used in a callback, the XMLParser is a thread-safe class as long as any given instance is only used in one thread.

Note

Namespace support was implemented in XMLParser starting in macOS 10.4. Namespace-related methods of XMLParser prior to this version have no effect.

## Topics

### Initializing a Parser Object

convenience init?(contentsOf: URL)

Initializes a parser with the XML content referenced by the given URL.

init(data: Data)

Initializes a parser with the XML contents encapsulated in a given data object.

convenience init(stream: InputStream)

Initializes a parser with the XML contents from the specified stream and parses it.

### Managing Delegates

var delegate: (any XMLParserDelegate)?

A delegate object that receives messages about the parsing process.

### Managing Parser Behavior

var shouldProcessNamespaces: Bool

A Boolean value that determines whether the parser reports the namespaces and qualified names of elements.

var shouldReportNamespacePrefixes: Bool

A Boolean value that determines whether the parser reports the prefixes indicating the scope of namespace declarations.

var shouldResolveExternalEntities: Bool

A Boolean value that determines whether the parser reports declarations of external entities.

### Parsing

func parse() -> Bool

Starts the event-driven parsing operation.

func abortParsing()

Stops the parser object.

var parserError: (any Error)?

An NSError object from which you can obtain information about a parsing error.

### Obtaining Parser State

var columnNumber: Int

The column number of the XML document being processed by the parser.

var lineNumber: Int

The line number of the XML document being processed by the parser.

var publicID: String?

The public identifier of the external entity referenced in the XML document.

var systemID: String?

The system identifier of the external entity referenced in the XML document.

### Constants

enum ExternalEntityResolvingPolicy

class let errorDomain: String

Indicates an error in XML parsing.

enum ErrorCode

The following error codes are defined by `NSXMLParser`. For error codes not listed here, see the `` header file.

### Instance Properties

var allowedExternalEntityURLs: Set&lt;URL>?

var externalEntityResolvingPolicy: XMLParser.ExternalEntityResolvingPolicy

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Event-Based Processing

protocol XMLParserDelegate

The interface an XML parser uses to inform its delegate about the content of the parsed document.

