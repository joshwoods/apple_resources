

- AppKit
- NSAccessibilityLayoutItem
-  setAccessibilityFrame(\_:) 

Instance Method

# setAccessibilityFrame(\_:)

Sets the accessibility element’s frame.

macOS

``` source
optional func setAccessibilityFrame(_ frame: NSRect)
```

## Parameters 

`frame`  

The new frame in screen coordinates.

## Discussion

This method is the setter method for the NSAccessibilityProtocol protocol’s accessibilityFrame property. By implementing this method, you allow accessibility clients to modify this element’s frame.

