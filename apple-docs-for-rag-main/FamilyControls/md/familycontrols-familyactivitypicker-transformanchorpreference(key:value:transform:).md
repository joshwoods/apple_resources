

- FamilyControls
- FamilyActivityPicker
-  transformAnchorPreference(key:value:transform:) 

Instance Method

# transformAnchorPreference(key:value:transform:)

Sets a value for the specified preference key, the value is a function of the key’s current value and a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func transformAnchorPreference(
    key _: K.Type = K.self,
    value: Anchor.Source,
    transform: @escaping (inout K.Value, Anchor) -> Void
) -> some View where K : PreferenceKey
```

## Parameters 

`key`  

The preference key type.

`value`  

The geometry value in the current coordinate space.

`transform`  

The function to produce the preference value.

## Return Value

A new version of the view that writes the preference.

## See Also

### Preferences

func preference&lt;K>(key: K.Type, value: K.Value) -> some View

Sets a value for the given preference.

func transformPreference&lt;K>(K.Type, (inout K.Value) -> Void) -> some View

Applies a transformation to a preference value.

func anchorPreference&lt;A, K>(key: K.Type, value: Anchor&lt;A>.Source, transform: (Anchor&lt;A>) -> K.Value) -> some View

Sets a value for the specified preference key, the value is a function of a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

func onPreferenceChange&lt;K>(K.Type, perform: (K.Value) -> Void) -> some View

Adds an action to perform when the specified preference key’s value changes.

func backgroundPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as the background of the original view.

func overlayPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as an overlay to the original view.

