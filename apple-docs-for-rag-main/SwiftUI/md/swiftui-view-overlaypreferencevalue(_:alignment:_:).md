

- SwiftUI
- View
-  overlayPreferenceValue(\_:alignment:\_:) 

Instance Method

# overlayPreferenceValue(\_:alignment:\_:)

Reads the specified preference value from the view, using it to produce a second view that is applied as an overlay to the original view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func overlayPreferenceValue(
    _ key: K.Type,
    alignment: Alignment = .center,
    @ViewBuilder _ transform: @escaping (K.Value) -> V
) -> some View where K : PreferenceKey, V : View
```

## Parameters 

`key`  

The preference key type whose value is to be read.

`alignment`  

An optional alignment to use when positioning the overlay view relative to the original view.

`transform`  

A function that produces the overlay view from the preference value read from the original view.

## Return Value

A view that layers a second view in front of the view.

## Discussion

The values of the preference key from both views are combined and made visible to the parent view.

## See Also

### Generating backgrounds and overlays from preferences

func backgroundPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as the background of the original view.

func backgroundPreferenceValue&lt;K, V>(K.Type, alignment: Alignment, (K.Value) -> V) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as the background of the original view.

func overlayPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as an overlay to the original view.

