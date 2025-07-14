

- SwiftUI
- View
-  symbolEffectsRemoved(\_:) 

Instance Method

# symbolEffectsRemoved(\_:)

Returns a new view with its inherited symbol image effects either removed or left unchanged.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func symbolEffectsRemoved(_ isEnabled: Bool = true) -> some View
```

## Parameters 

`isEnabled`  

Whether to remove inherited symbol effects or not.

## Return Value

A copy of the view with its symbol effects either removed or left unchanged.

## Discussion

The following example adds a repeating pulse effect to two symbol images, but then disables the effect on one of them:

```
VStack {
    Image(systemName: "bolt.slash.fill") // does not pulse
        .symbolEffectsRemoved()
    Image(systemName: "folder.fill.badge.person.crop") // pulses
}
.symbolEffect(.pulse)
```

## See Also

### Managing symbol effects

func symbolEffect&lt;T>(T, options: SymbolEffectOptions, isActive: Bool) -> some View

Returns a new view with a symbol effect added to it.

func symbolEffect&lt;T, U>(T, options: SymbolEffectOptions, value: U) -> some View

Returns a new view with a symbol effect added to it.

struct SymbolEffectTransition

Creates a transition that applies the Appear or Disappear symbol animation to symbol images within the inserted or removed view hierarchy.

