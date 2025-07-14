

- MusicKit
- ArtworkImage
-  windowDismissBehavior(\_:) 

Instance Method

# windowDismissBehavior(\_:)

Configures the dismiss functionality for the window enclosing `self`.

MusicKitSwiftUImacOS 15.0+

``` source
nonisolated
func windowDismissBehavior(_ behavior: WindowInteractionBehavior) -> some View
```

## Parameters 

`behavior`  

The dismiss behavior.

## Discussion

By default, the window dismiss functionality is determined by the scene, as well as any modifiers applied to it.

You can use this modifier to override the default behavior.

For example, you can create a welcome workflow window which disables the dismiss functionality:

```
struct MyApp: App {
    var body: some Scene {
        ...
        Window("Welcome", id: "welcome") {
            WelcomeView()
                .windowDismissBehavior(.disabled)
        }
    }
}
```

