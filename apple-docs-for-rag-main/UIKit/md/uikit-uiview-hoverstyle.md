

- UIKit
- UIView
-  hoverStyle 

Instance Property

# hoverStyle

The hover style for the view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var hoverStyle: UIHoverStyle? { get set }
```

## Discussion

The value of this property defaults to `nil`, which indicates that the view doesn’t have any hover effect. Subclasses can configure this style to use a different default value.

## See Also

### Managing the hover appearance

class UIHoverStyle

The hover style to apply to a view, including an effect and a shape to use for displaying that effect.

class UIHoverEffectLayer

