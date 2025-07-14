

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXProxyAttribute 

Global Variable

# kAXProxyAttribute

macOS 10.2+

``` source
var kAXProxyAttribute: String { get }
```

## Discussion

The document proxy of the window represented by this accessibility object. An accessibility object includes this attribute to help an assistive application easily find a window’s document proxy, without having to traverse the accessibility hierarchy. This attribute is recommended for all accessibility objects that represent windows that display a document proxy.

