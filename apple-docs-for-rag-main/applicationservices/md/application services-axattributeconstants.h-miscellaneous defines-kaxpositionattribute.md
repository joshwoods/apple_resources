

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXPositionAttribute 

Global Variable

# kAXPositionAttribute

macOS 10.2+

``` source
var kAXPositionAttribute: String { get }
```

## Discussion

The global screen coordinates of the top-left corner of this accessibility object. Note that the coordinates `0`,`0` represent the top-left corner of the screen that displays the menu bar. All accessibility objects that have a screen position (in other words, are visible on the screen) should include this attribute.

