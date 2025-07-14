

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXHeaderAttribute 

Global Variable

# kAXHeaderAttribute

macOS 10.2+

``` source
var kAXHeaderAttribute: String { get }
```

## Discussion

The accessibility object representing the header element of this accessibility object. For example, a table or an outline view can have a header element that displays column or row headers. An accessibility object includes this attribute to help an assistive application easily find embedded header information. This attribute is recommended for all accessibility objects that represent elements that display header information.

