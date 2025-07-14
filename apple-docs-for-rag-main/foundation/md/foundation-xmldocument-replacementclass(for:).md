

- Foundation
- XMLDocument
-  replacementClass(for:) 

Type Method

# replacementClass(for:)

Overridden by subclasses to substitute a custom class for an NSXML class that the parser uses to create node instances.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func replacementClass(for cls: AnyClass) -> AnyClass
```

## Parameters 

`cls`  

A `Class` object identifying an NSXML class that is to be replaced by your custom class.

## Return Value

The substituted class.

## Discussion

For example, if you have a custom subclass of XMLElement that you want to be used in place of `NSXMLElement`, you would make the following override:

```
+ (Class)replacementClassForClass:(Class)currentClass {
    if ( currentClass == [NSXMLElement class] ) {
        return [MyCustomElementClass class];
    }
}
```

This method is invoked before a document is parsed. The substituted class must be a subclass of XMLNode, `NSXMLDocument`, `NSXMLElement`, XMLDTD, or XMLDTDNode.

## See Also

### Related Documentation

func setRootElement(XMLElement)

Set the root element of the receiver.

### Initializing NSXMLDocument Objects

convenience init(contentsOf: URL, options: XMLNode.Options) throws

Initializes and returns an NSXMLDocument object created from the XML or HTML contents of a URL-referenced source

init(data: Data, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDocument` object created from an NSData object.

init(rootElement: XMLElement?)

Returns an `NSXMLDocument` object initialized with a single child, the root element.

convenience init(xmlString: String, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDocument` object created from a string containing XML markup text.

