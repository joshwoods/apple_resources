

- FamilyControls
- FamilyActivityPicker
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

## See Also

### Preferences

func preference&lt;K>(key: K.Type, value: K.Value) -> some View

Sets a value for the given preference.

func transformPreference&lt;K>(K.Type, (inout K.Value) -> Void) -> some View

Applies a transformation to a preference value.

func anchorPreference&lt;A, K>(key: K.Type, value: Anchor&lt;A>.Source, transform: (Anchor&lt;A>) -> K.Value) -> some View

Sets a value for the specified preference key, the value is a function of a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

func transformAnchorPreference&lt;A, K>(key: K.Type, value: Anchor&lt;A>.Source, transform: (inout K.Value, Anchor&lt;A>) -> Void) -> some View

Sets a value for the specified preference key, the value is a function of the key’s current value and a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

func onPreferenceChange&lt;K>(K.Type, perform: (K.Value) -> Void) -> some View

Adds an action to perform when the specified preference key’s value changes.

func backgroundPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as the background of the original view.

