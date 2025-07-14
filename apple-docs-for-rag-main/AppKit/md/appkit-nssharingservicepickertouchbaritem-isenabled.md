

- AppKit
- NSSharingServicePickerTouchBarItem
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that specifies whether the sharing service picker item is enabled.

macOS 10.12.2+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

If true, the sharing button is enabled.

If the sharing popover is currently visible when this property is changed to false, the popover is dismissed.

