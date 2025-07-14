

- SwiftUI
- View
-  transformAnchorPreference(key:value:transform:) 

Instance Method

# transformAnchorPreference(key:value:transform:)

Sets a value for the specified preference key, the value is a function of the key’s current value and a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

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

### Setting preferences based on geometry

func anchorPreference&lt;A, K>(key: K.Type, value: Anchor&lt;A>.Source, transform: (Anchor&lt;A>) -> K.Value) -> some View

Sets a value for the specified preference key, the value is a function of a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

