

- ManagedAppDistribution
- ManagedContentView
-  anchorPreference(key:value:transform:) 

Instance Method

# anchorPreference(key:value:transform:)

Sets a value for the specified preference key, the value is a function of a geometry value tied to the current coordinate space, allowing readers of the value to convert the geometry to their local coordinates.

ManagedAppDistributionSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func anchorPreference(
    key _: K.Type = K.self,
    value: Anchor.Source,
    transform: @escaping (Anchor) -> K.Value
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

