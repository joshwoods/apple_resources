

- SwiftUI
- CustomHoverEffect
-  automatic 

Type Property

# automatic

The default hover effect based on the surrounding context.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
static var automatic: AutomaticHoverEffect { get }
```

Available when `Self` is `AutomaticHoverEffect`.

## Discussion

The automatic effect will resolve to any defaultHoverEffect(_:) applied to the current View hierarchy, or a system-defined effect if no default effect has been defined.

## See Also

### Getting built-in hover effects

static var empty: EmptyHoverEffect

An effect that applies no changes when hovered.

static var highlight: HighlightHoverEffect

A hover effect that highlights views using a light source to indicate position.

static var lift: LiftHoverEffect

A hover effect that slides the pointer under the view and disappears as the view scales up and gains a shadow.

