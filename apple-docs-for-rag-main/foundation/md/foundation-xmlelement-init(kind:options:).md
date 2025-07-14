

- Foundation
- XMLElement
-  init(kind:options:) 

Initializer

# init(kind:options:)

Mac Catalyst 13.0+macOS 10.0+

``` source
convenience init(
    kind: XMLNode.Kind,
    options: XMLNode.Options = []
)
```

## See Also

### Initializing NSXMLElement Objects

convenience init(name: String)

Returns an `NSXMLElement` object initialized with the specified name.

convenience init(name: String, stringValue: String?)

Returns an `NSXMLElement` object initialized with a specified name and a single text-node child containing a specified value.

init(name: String, uri: String?)

Returns an `NSXMLElement` object initialized with the specified name and URI.

init(xmlString: String) throws

Returns an `NSXMLElement` object created from a specified string containing XML markup.

