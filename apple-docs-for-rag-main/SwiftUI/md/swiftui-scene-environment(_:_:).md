

- SwiftUI
- Scene
-  environment(\_:\_:) 

Instance Method

# environment(\_:\_:)

Sets the environment value of the specified key path to the given value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func environment(
    _ keyPath: WritableKeyPath,
    _ value: V
) -> some Scene
```

## Parameters 

`keyPath`  

A key path that indicates the property of the EnvironmentValues structure to update.

`value`  

The new value to set for the item specified by `keyPath`.

## Return Value

A view that has the given value set in its environment.

## Discussion

Use this modifier to set one of the writable properties of the EnvironmentValues structure, including custom values that you create. For example, you can create a custom environment key `styleOverrides` to set a value that represents style settings that for the entire app:

```
WindowGroup {
    ContentView()
}
.environment(\.styleOverrides, StyleOverrides())
```

You then read the value inside `ContentView` or one of its descendants using the Environment property wrapper:

```
struct MyView: View {
    @Environment(\.styleOverrides) var styleOverrides: StyleOverrides

    var body: some View { ... }
}
```

This modifier affects the given scene, as well as that scene’s descendant views. It has no effect outside the view hierarchy on which you call it.

## See Also

### Modifying the environment of a scene

func environment&lt;T>(T?) -> some Scene

Places an observable object in the scene’s environment.

func transformEnvironment&lt;V>(WritableKeyPath&lt;EnvironmentValues, V>, transform: (inout V) -> Void) -> some Scene

Transforms the environment value of the specified key path with the given function.

