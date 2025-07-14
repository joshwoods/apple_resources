

- Foundation
- XMLElement
-  init(name:uri:) 

Initializer

# init(name:uri:)

Returns an `NSXMLElement` object initialized with the specified name and URI.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    name: String,
    uri URI: String?
)
```

## Parameters 

`name`  

A string that specifies the qualified name of the element.

`URI`  

A string that specifies the namespace URI associated with the element.

## Return Value

The initialized `NSXMLElement` object or `nil` if initialization did not succeed.

## Discussion

You can look up the namespace prefix for this element node based on its URI using resolvePrefix(forNamespaceURI:). This method is the primary initializer for the `NSXMLElement` class.

## See Also

### Initializing NSXMLElement Objects

convenience init(name: String)

Returns an `NSXMLElement` object initialized with the specified name.

convenience init(name: String, stringValue: String?)

Returns an `NSXMLElement` object initialized with a specified name and a single text-node child containing a specified value.

init(xmlString: String) throws

Returns an `NSXMLElement` object created from a specified string containing XML markup.

convenience init(kind: XMLNode.Kind, options: XMLNode.Options)

