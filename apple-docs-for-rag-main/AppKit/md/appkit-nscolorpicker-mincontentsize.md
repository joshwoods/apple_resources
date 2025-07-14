

- AppKit
- NSColorPicker
-  minContentSize 

Instance Property

# minContentSize

The minimum content size.

macOS

``` source
var minContentSize: NSSize { get }
```

## Discussion

The containing NSColorPanel object does not allow the color picker to be made smaller than this size.

Override this property’s getter method to return a minimum size for the color picker’s content area. The default implementation obtains the minimum content size from the view-autoresizing behavior specified for the color picker. You should not have to override this method if you properly set up the color picker’s auto-sizing attributes in Interface Builder.

## See Also

### Customizing the Color Picker

var buttonToolTip: String

The tool tip that is shown when the mouse cursor is over the color picker’s button image.

