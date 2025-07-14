

- App Intents
- ShortcutsLink
-  transformEnvironment(\_:transform:) 

Instance Method

# transformEnvironment(\_:transform:)

Transforms the environment value of the specified key path with the given function.

AppIntentsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func transformEnvironment(
    _ keyPath: WritableKeyPath,
    transform: @escaping (inout V) -> Void
) -> some View
```

