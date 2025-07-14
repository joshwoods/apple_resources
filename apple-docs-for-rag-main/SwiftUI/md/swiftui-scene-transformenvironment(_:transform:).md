

- SwiftUI
- Scene
-  transformEnvironment(\_:transform:) 

Instance Method

# transformEnvironment(\_:transform:)

Transforms the environment value of the specified key path with the given function.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func transformEnvironment(
    _ keyPath: WritableKeyPath,
    transform: @escaping (inout V) -> Void
) -> some Scene
```

## See Also

### Modifying the environment of a scene

func environment&lt;T>(T?) -> some Scene

Places an observable object in the scene’s environment.

func environment&lt;V>(WritableKeyPath&lt;EnvironmentValues, V>, V) -> some Scene

Sets the environment value of the specified key path to the given value.

