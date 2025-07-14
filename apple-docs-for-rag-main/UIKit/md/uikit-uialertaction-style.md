

- UIKit
- UIAlertAction
-  style 

Instance Property

# style

The style that applies to the action’s button.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var style: UIAlertAction.Style { get }
```

## Discussion

This property is set to the value you specified in the init(title:style:handler:) method.

## See Also

### Getting the action’s attributes

var title: String?

The title of the action’s button.

var isEnabled: Bool

A Boolean value indicating whether the action is currently enabled.

