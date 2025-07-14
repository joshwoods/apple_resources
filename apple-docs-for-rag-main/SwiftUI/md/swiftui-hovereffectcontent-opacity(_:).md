

- SwiftUI
- HoverEffectContent
-  opacity(\_:) 

Instance Method

# opacity(\_:)

Sets the transparency of the view.

visionOS 2.0+

``` source
func opacity(_ opacity: Double) -> some HoverEffectContent
```

## Parameters 

`opacity`  

A value between 0 (fully transparent) and 1 (fully opaque).

## Return Value

An effect that sets the transparency of the view.

## Discussion

When applying the `opacity(_:)` effect to a view that has already had its opacity transformed, the effect of the underlying opacity transformation is multiplied.

