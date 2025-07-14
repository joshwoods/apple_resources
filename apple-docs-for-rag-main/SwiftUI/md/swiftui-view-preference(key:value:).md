

- SwiftUI
- View
-  preference(key:value:) 

Instance Method

# preference(key:value:)

Sets a value for the given preference.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func preference(
    key: K.Type = K.self,
    value: K.Value
) -> some View where K : PreferenceKey
```

## See Also

### Setting preferences

func transformPreference&lt;K>(K.Type, (inout K.Value) -> Void) -> some View

Applies a transformation to a preference value.

