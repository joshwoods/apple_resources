

- RealityKit
- RealityViewAttachmentBuilderContent
-  environment(\_:\_:) 

Instance Method

# environment(\_:\_:)

Sets the environment value of the specified key path to the given value.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func environment(
    _ keyPath: WritableKeyPath,
    _ value: V
) -> some View
```

## Parameters 

`keyPath`  

A key path that indicates the property of the `EnvironmentValues` structure to update.

`value`  

The new value to set for the item specified by `keyPath`.

## Return Value

A view that has the given value set in its environment.

## Discussion

Use this modifier to set one of the writable properties of the `EnvironmentValues` structure, including custom values that you create. For example, you can set the value associated with the `EnvironmentValues/truncationMode` key:

```
MyView()
    .environment(\.truncationMode, .head)
```

You then read the value inside `MyView` or one of its descendants using the `Environment` property wrapper:

```
struct MyView: View {
    @Environment(\.truncationMode) var truncationMode: Text.TruncationMode

    var body: some View { ... }
}
```

SwiftUI provides dedicated view modifiers for setting most environment values, like the `View/truncationMode(_:)` modifier which sets the `EnvironmentValues/truncationMode` value:

```
MyView()
    .truncationMode(.head)
```

Prefer the dedicated modifier when available, and offer your own when defining custom environment values, as described in `Entry()`.

This modifier affects the given view, as well as that view’s descendant views. It has no effect outside the view hierarchy on which you call it.

