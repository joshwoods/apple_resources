

- Foundation
- XMLParser
-  init(data:) 

Initializer

# init(data:)

Initializes a parser with the XML contents encapsulated in a given data object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(data: Data)
```

## Parameters 

`data`  

An NSData object containing XML markup.

## Return Value

An initialized `NSXMLParser` object or `nil` if an error occurs.

## Discussion

This method is the designated initializer.

## See Also

### Initializing a Parser Object

convenience init?(contentsOf: URL)

Initializes a parser with the XML content referenced by the given URL.

convenience init(stream: InputStream)

Initializes a parser with the XML contents from the specified stream and parses it.

