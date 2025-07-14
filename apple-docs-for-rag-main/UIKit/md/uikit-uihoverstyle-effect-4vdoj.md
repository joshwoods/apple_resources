

- UIKit
- UIHoverStyle
-  effect 

Instance Property

# effect

The effect to apply to the view with this style.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS 1.0+

``` source
@MainActor @preconcurrency
var effect: any UIHoverEffect { get set }
```

## Discussion

Use UIHoverAutomaticEffect to apply a system-default effect to the view.

## See Also

### Specifying a hover effect

struct UIHoverAutomaticEffect

A system-default hover effect that automatically selects the appropriate effect based on the view to which it applies.

struct UIHoverHighlightEffect

An effect that applies a highlight to the view on hover.

struct UIHoverLiftEffect

An effect that can visually lift the view on hover where appropriate.

protocol UIHoverEffect

A hover effect that can apply to a view through a hover style.

