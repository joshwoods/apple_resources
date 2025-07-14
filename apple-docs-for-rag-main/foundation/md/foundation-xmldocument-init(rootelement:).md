

- Foundation
- XMLDocument
-  init(rootElement:) 

Initializer

# init(rootElement:)

Returns an `NSXMLDocument` object initialized with a single child, the root element.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(rootElement element: XMLElement?)
```

## Parameters 

`element`  

An XMLElement object representing an XML element.

## Return Value

An initialized `NSXMLDocument` object, or `nil` if initialization fails for any reason.

## See Also

### Initializing NSXMLDocument Objects

convenience init(contentsOf: URL, options: XMLNode.Options) throws

Initializes and returns an NSXMLDocument object created from the XML or HTML contents of a URL-referenced source

init(data: Data, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDocument` object created from an NSData object.

convenience init(xmlString: String, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDocument` object created from a string containing XML markup text.

class func replacementClass(for: AnyClass) -> AnyClass

Overridden by subclasses to substitute a custom class for an NSXML class that the parser uses to create node instances.

