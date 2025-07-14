

- AppKit
- NSSliderTouchBarItem
-  target 

Instance Property

# target

An object that is notified when a user interacts with the slider or either of the accessories.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
weak var target: AnyObject? { get set }
```

## See Also

### Handling slider interaction

var action: Selector?

The selector on the target object that is invoked when a user interacts with the slider or either of the accessories.

