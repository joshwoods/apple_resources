

- RealityKit
- Model3D
-  monospaced(\_:) 

Instance Method

# monospaced(\_:)

Modifies the fonts of all child views to use the fixed-width variant of the current font, if possible.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
func monospaced(_ isActive: Bool = true) -> some View
```

## Return Value

A view whose child views’ fonts use fixed-width characters, while leaving other characters proportionally spaced.

## Discussion

If a child view’s base font doesn’t support fixed-width, the font remains unchanged.

