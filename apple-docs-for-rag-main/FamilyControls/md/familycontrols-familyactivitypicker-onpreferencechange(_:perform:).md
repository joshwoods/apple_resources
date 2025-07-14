

- FamilyControls
- FamilyActivityPicker
-  onPreferenceChange(\_:perform:) 

Instance Method

# onPreferenceChange(\_:perform:)

Adds an action to perform when the specified preference key’s value changes.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func onPreferenceChange(
    _ key: K.Type = K.self,
    perform action: @escaping (K.Value) -> Void
) -> some View where K : PreferenceKey, K.Value : Equatable
```

## Parameters 

`key`  

The key to monitor for value changes.

`action`  

The action to perform when the value for `key` changes. The `action` closure passes the new value as its parameter.

## Return Value

A view that triggers `action` when the value for `key` changes.

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

func backgroundPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as the background of the original view.

func overlayPreferenceValue&lt;Key, T>(Key.Type, (Key.Value) -> T) -> some View

Reads the specified preference value from the view, using it to produce a second view that is applied as an overlay to the original view.

