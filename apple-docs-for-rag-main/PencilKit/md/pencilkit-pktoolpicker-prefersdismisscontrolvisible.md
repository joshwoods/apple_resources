

- PencilKit
- PKToolPicker
-  prefersDismissControlVisible 

Instance Property

# prefersDismissControlVisible

If this is true the tool picker may show UI that allows dismissing it. If this is false the tool picker will not show this UI. By default this resigns first responder, but is customizable by `PKToolPickerDelegate`’s `toolPickerWillDismiss...` method.

visionOS 2.0+

``` source
var prefersDismissControlVisible: Bool { get set }
```

## Discussion

By default this is true.

