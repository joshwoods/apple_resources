

- AppKit
- NSColorPickerTouchBarItem
-  target 

Instance Property

# target

An object that is notified when a user interacts with the color picker.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
weak var target: AnyObject? { get set }
```

## See Also

### Obtaining the selected color

var color: UIColor

The picker’s currently selected color.

var action: Selector?

The selector on the target object that is invoked when a user interacts with the color picker.

