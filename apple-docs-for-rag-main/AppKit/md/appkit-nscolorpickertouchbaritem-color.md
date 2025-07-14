

- AppKit
- NSColorPickerTouchBarItem
-  color 

Instance Property

# color

The picker’s currently selected color.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

**macOS**

``` source
@NSCopying @MainActor
var color: NSColor { get set }
```

**Mac Catalyst**

``` source
@NSCopying @MainActor
var color: UIColor { get set }
```

## See Also

### Obtaining the selected color

var target: AnyObject?

An object that is notified when a user interacts with the color picker.

var action: Selector?

The selector on the target object that is invoked when a user interacts with the color picker.

