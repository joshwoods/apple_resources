

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXTopLevelUIElementAttribute 

Global Variable

# kAXTopLevelUIElementAttribute

macOS 10.4+

``` source
var kAXTopLevelUIElementAttribute: String { get }
```

## Discussion

The window, sheet, or drawer element that contains this accessibility object. An accessibility object that is contained in a window, sheet, or drawer includes this attribute so an assistive application easily can find that element without having to step through all intervening objects in the accessibility hierarchy. This attribute is required for all accessibility objects whose parent or more distant ancestor represents a window, drawer, or sheet.

