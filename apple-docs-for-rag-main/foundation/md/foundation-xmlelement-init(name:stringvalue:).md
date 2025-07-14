

- Foundation
- XMLElement
-  init(name:stringValue:) 

Initializer

# init(name:stringValue:)

Returns an `NSXMLElement` object initialized with a specified name and a single text-node child containing a specified value.

Mac Catalyst 13.0+macOS 10.0+

``` source
convenience init(
    name: String,
    stringValue string: String?
)
```

## Parameters 

`name`  

A string specifying the name of the element.

`string`  

The string value of the receiver’s text node.

## Return Value

The initialized `NSXMLElement` object or `nil` if initialization did not succeed.

## Discussion

The string representation of this object is ``` ``string`` ```.

## See Also

### Initializing NSXMLElement Objects

convenience init(name: String)

Returns an `NSXMLElement` object initialized with the specified name.

init(name: String, uri: String?)

Returns an `NSXMLElement` object initialized with the specified name and URI.

init(xmlString: String) throws

Returns an `NSXMLElement` object created from a specified string containing XML markup.

convenience init(kind: XMLNode.Kind, options: XMLNode.Options)

