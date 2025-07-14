

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  accessibilityIgnoresInvertColors(\_:) 

Instance Method

# accessibilityIgnoresInvertColors(\_:)

Sets whether this view should ignore the system Smart Invert setting.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
nonisolated
func accessibilityIgnoresInvertColors(_ active: Bool = true) -> some View
```

## Parameters 

`active`  

A true value ignores the system Smart Invert setting. A false value follows the system setting.

## Discussion

Use this modifier to suppress Smart Invert in a view that shouldn’t be inverted. Or pass an `active` argument of `false` to begin following the Smart Invert setting again when it was previously disabled.

