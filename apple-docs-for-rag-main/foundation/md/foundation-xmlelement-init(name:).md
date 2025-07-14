

- Foundation
- XMLElement
-  init(name:) 

Initializer

# init(name:)

Returns an `NSXMLElement` object initialized with the specified name.

Mac Catalyst 13.0+macOS 10.0+

``` source
convenience init(name: String)
```

## Parameters 

`name`  

A string specifying the name of the element.

## Return Value

The initialized `NSXMLElement` object or `nil` if initialization did not succeed.

## Discussion

The XML string representation of this object is ```  ```. This method invokes init(name:uri:) with the URI parameter set to `nil`.

## See Also

### Related Documentation

Tree-Based XML Programming Guide

### Initializing NSXMLElement Objects

convenience init(name: String, stringValue: String?)

Returns an `NSXMLElement` object initialized with a specified name and a single text-node child containing a specified value.

init(name: String, uri: String?)

Returns an `NSXMLElement` object initialized with the specified name and URI.

init(xmlString: String) throws

Returns an `NSXMLElement` object created from a specified string containing XML markup.

convenience init(kind: XMLNode.Kind, options: XMLNode.Options)

