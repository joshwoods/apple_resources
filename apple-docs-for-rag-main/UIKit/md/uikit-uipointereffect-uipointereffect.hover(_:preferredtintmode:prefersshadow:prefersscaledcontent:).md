

- UIKit
- UIPointerEffect
-  UIPointerEffect.hover(\_:preferredTintMode:prefersShadow:prefersScaledContent:) 

Case

# UIPointerEffect.hover(\_:preferredTintMode:prefersShadow:prefersScaledContent:)

An effect where visual changes apply to the view and the pointer retains its default shape.

iOS 13.4+iPadOS 13.4+Mac CatalystvisionOS

``` source
case hover(
    UITargetedPreview,
    preferredTintMode: UIPointerEffect.TintMode = .overlay,
    prefersShadow: Bool = false,
    prefersScaledContent: Bool = true
)
```

## Topics

### Specifying the Tint Mode

enum TintMode

An effect that defines how to apply a tint to a view during a pointer interaction.

## See Also

### Creating a specific effect

case highlight(UITargetedPreview)

An effect where the pointer slides under the given view and morphs into the view’s shape.

case lift(UITargetedPreview)

An effect where the pointer slides under the given view and disappears as the view scales up and gains a shadow.

