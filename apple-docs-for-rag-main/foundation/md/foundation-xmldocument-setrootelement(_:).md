

- Foundation
- XMLDocument
-  setRootElement(\_:) 

Instance Method

# setRootElement(\_:)

Set the root element of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setRootElement(_ root: XMLElement)
```

## Parameters 

`root`  

An XMLNode object that is to be the root element.

## Discussion

As a side effect, this method removes all other children, including `NSXMLNode` objects representing comments and processing-instructions.

## See Also

### Managing the Root Element

func rootElement() -> XMLElement?

Returns the root element of the receiver.

