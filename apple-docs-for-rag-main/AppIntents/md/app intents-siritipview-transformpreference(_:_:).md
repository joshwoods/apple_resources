

- App Intents
- SiriTipView
-  transformPreference(\_:\_:) 

Instance Method

# transformPreference(\_:\_:)

Applies a transformation to a preference value.

AppIntentsSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func transformPreference(
    _ key: K.Type = K.self,
    _ callback: @escaping (inout K.Value) -> Void
) -> some View where K : PreferenceKey
```

