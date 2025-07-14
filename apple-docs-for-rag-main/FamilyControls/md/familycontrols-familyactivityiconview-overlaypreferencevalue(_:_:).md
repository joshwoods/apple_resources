

- FamilyControls
- FamilyActivityIconView
-  overlayPreferenceValue(\_:\_:) 

Instance Method

# overlayPreferenceValue(\_:\_:)

Reads the specified preference value from the view, using it to produce a second view that is applied as an overlay to the original view.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func overlayPreferenceValue(
    _ key: Key.Type = Key.self,
    @ViewBuilder _ transform: @escaping (Key.Value) -> T
) -> some View where Key : PreferenceKey, T : View
```

## Parameters 

`key`  

The preference key type whose value is to be read.

`transform`  

A function that produces the overlay view from the preference value read from the original view.

## Return Value

A view that layers a second view in front of the view.

