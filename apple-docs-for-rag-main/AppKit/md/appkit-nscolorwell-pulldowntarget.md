

- AppKit
- NSColorWell
-  pulldownTarget 

Instance Property

# pulldownTarget

The target object that defines the action you want to perform when someone interacts with the color well.

macOS 13.0+

``` source
@MainActor
weak var pulldownTarget: AnyObject? { get set }
```

## Discussion

Specify a custom action method to replace the system popover and color picker. For a color well with the NSColorWell.Style.minimal or NSColorWell.Style.expanded style, clicks in the color area normally display a popover with the system color picker. If you specify a value for this property and the pulldownAction property, clicks in the color area execute your custom action method instead.

## See Also

### Customizing the Color Selection Behavior

var pulldownAction: Selector?

The action to perform when someone clicks in the color area of the color well.

