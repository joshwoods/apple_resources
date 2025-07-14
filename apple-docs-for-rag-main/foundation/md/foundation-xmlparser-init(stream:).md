

- Foundation
- XMLParser
-  init(stream:) 

Initializer

# init(stream:)

Initializes a parser with the XML contents from the specified stream and parses it.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(stream: InputStream)
```

## Parameters 

`stream`  

The input stream. The content is incrementally loaded from the specified stream and parsed. The `NSXMLParser` will open the stream, and synchronously read from it without scheduling it.

## Return Value

An initialized `NSXMLParser` object or `nil` if an error occurs.

## See Also

### Initializing a Parser Object

convenience init?(contentsOf: URL)

Initializes a parser with the XML content referenced by the given URL.

init(data: Data)

Initializes a parser with the XML contents encapsulated in a given data object.

