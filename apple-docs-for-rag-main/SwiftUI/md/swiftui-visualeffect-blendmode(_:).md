

- SwiftUI
- VisualEffect
-  blendMode(\_:) 

Instance Method

# blendMode(\_:)

Sets the blend mode for compositing this view with overlapping views.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func blendMode(_ blendMode: BlendMode) -> some VisualEffect
```

## Parameters 

`blendMode`  

The BlendMode for compositing.

## Return Value

An effect that applies `blendMode` to this view.

## Discussion

Use `blendMode(_:)` to combine overlapping views and use a different visual effect to produce the result. The BlendMode enumeration defines many possible effects.

