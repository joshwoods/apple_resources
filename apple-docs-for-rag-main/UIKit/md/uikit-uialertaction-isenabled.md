

- UIKit
- UIAlertAction
-  isEnabled 

Instance Property

# isEnabled

A Boolean value indicating whether the action is currently enabled.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

The default value of this property is true. Changing the value to false causes the action to appear dimmed in the resulting alert. When an action is disabled, taps on the corresponding button have no effect.

## See Also

### Getting the action’s attributes

var title: String?

The title of the action’s button.

var style: UIAlertAction.Style

The style that applies to the action’s button.

