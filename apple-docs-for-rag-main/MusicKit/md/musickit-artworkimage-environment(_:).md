

- MusicKit
- ArtworkImage
-  environment(\_:) 

Instance Method

# environment(\_:)

Places an observable object in the view’s environment.

MusicKitSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func environment(_ object: T?) -> some View where T : AnyObject, T : Observable
```

## Parameters 

`object`  

The object to set for this object’s type in the environment, or `nil` to clear an object of this type from the environment.

## Return Value

A view that has the specified object in its environment.

## Discussion

Use this modifier to place an object that you declare with the Observable() macro into a view’s environment. For example, you can add an instance of a custom observable `Profile` class to the environment of a `ContentView`:

```
@Observable class Profile { ... }

struct RootView: View {
    @State private var currentProfile: Profile?

    var body: some View {
        ContentView()
            .environment(currentProfile)
    }
}
```

You then read the object inside `ContentView` or one of its descendants using the `Environment` property wrapper:

```
struct ContentView: View {
    @Environment(Profile.self) private var currentProfile: Profile

    var body: some View { ... }
}
```

This modifier affects the given view, as well as that view’s descendant views. It has no effect outside the view hierarchy on which you call it. The environment of a given view hierarchy holds only one observable object of a given type.

Note

This modifier takes an object that conforms to the Observable protocol. To add environment objects that conform to the ObservableObject protocol, use `View/environmentObject(_:)` instead.

