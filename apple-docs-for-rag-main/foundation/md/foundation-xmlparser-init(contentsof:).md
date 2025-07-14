

- Foundation
- XMLParser
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Initializes a parser with the XML content referenced by the given URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(contentsOf url: URL)
```

## Parameters 

`url`  

An NSURL object specifying a URL. The URL must be fully qualified and refer to a scheme that is supported by the `NSURL` class.

## Return Value

An initialized `NSXMLParser` object or `nil` if an error occurs.

## See Also

### Related Documentation

Event-Driven XML Programming Guide

### Initializing a Parser Object

init(data: Data)

Initializes a parser with the XML contents encapsulated in a given data object.

convenience init(stream: InputStream)

Initializes a parser with the XML contents from the specified stream and parses it.

