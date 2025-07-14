

- Assignables
- AssignedWorkDocumentView
-  symbolEffect(\_:options:isActive:) 

Instance Method

# symbolEffect(\_:options:isActive:)

Returns a new view with a symbol effect added to it.

AssignablesSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
nonisolated
func symbolEffect(
    _ effect: T,
    options: SymbolEffectOptions = .default,
    isActive: Bool = true
) -> some View where T : IndefiniteSymbolEffect, T : SymbolEffect
```

## Parameters 

`effect`  

A symbol effect to add to the view. Existing effects added by ancestors of the view are preserved, but may be overridden by the new effect. Added effects will be applied to the \`\`SwiftUI/Image\` views contained by the child view.

`isActive`  

Whether the effect is active or inactive.

## Return Value

A copy of the view with a symbol effect added.

## Discussion

The following example adds a repeating pulse effect to two symbol images:

```
VStack {
    Image(systemName: "bolt.slash.fill")
    Image(systemName: "folder.fill.badge.person.crop")
}
.symbolEffect(.pulse)
```

