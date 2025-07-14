

- RealityKit
- ObjectCapturePointCloudView
-  symbolEffect(\_:options:value:) 

Instance Method

# symbolEffect(\_:options:value:)

Returns a new view with a symbol effect added to it.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
func symbolEffect(
    _ effect: T,
    options: SymbolEffectOptions = .default,
    value: U
) -> some View where T : DiscreteSymbolEffect, T : SymbolEffect, U : Equatable
```

## Parameters 

`effect`  

A symbol effect to add to the view. Existing effects added by ancestors of the view are preserved, but may be overridden by the new effect. Added effects will be applied to the \`\`SwiftUI/Image\` views contained by the child view.

`value`  

The value to monitor for changes, the animation is triggered each time the value changes.

## Return Value

A copy of the view with a symbol effect added.

## Discussion

The following example adds a bounce effect to two symbol images, the animation will play each time `counter` changes:

```
VStack {
    Image(systemName: "bolt.slash.fill")
    Image(systemName: "folder.fill.badge.person.crop")
}
.symbolEffect(.bounce, value: counter)
```

