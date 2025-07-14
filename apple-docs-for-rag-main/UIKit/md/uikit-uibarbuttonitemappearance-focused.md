

- UIKit
- UIBarButtonItemAppearance
-  focused 

Instance Property

# focused

The appearance data to apply to the button when it’s focused.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var focused: UIBarButtonItemStateAppearance { get }
```

## Discussion

To set the attributes for this state, get the object in this property and modify it.

## See Also

### Configuring attributes for different button states

var normal: UIBarButtonItemStateAppearance

The appearance data to apply to the button when it’s in the normal state.

var disabled: UIBarButtonItemStateAppearance

The appearance data to apply to the button when it’s in the disabled state.

var highlighted: UIBarButtonItemStateAppearance

The appearance data to apply to the button when it’s in the highlighted state.

