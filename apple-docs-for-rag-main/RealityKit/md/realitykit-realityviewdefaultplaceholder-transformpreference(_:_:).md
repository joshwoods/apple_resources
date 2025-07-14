

- RealityKit
- RealityViewDefaultPlaceholder
-  transformPreference(\_:\_:) 

Instance Method

# transformPreference(\_:\_:)

Applies a transformation to a preference value.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func transformPreference(
    _ key: K.Type = K.self,
    _ callback: @escaping (inout K.Value) -> Void
) -> some View where K : PreferenceKey
```

