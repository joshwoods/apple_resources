

- SwiftUI
- Menu
-  init(\_:) 

Initializer

# init(\_:)

Creates a menu based on a style configuration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(_ configuration: MenuStyleConfiguration)
```

Available when `Label` is `MenuStyleConfiguration.Label` and `Content` is `MenuStyleConfiguration.Content`.

## Discussion

Use this initializer within the makeBody(configuration:) method of a MenuStyle instance to create an instance of the menu being styled. This is useful for custom menu styles that modify the current menu style.

For example, the following code creates a new, custom style that adds a red border around the current menu style:

```
struct RedBorderMenuStyle: MenuStyle {
    func makeBody(configuration: Configuration) -> some View {
        Menu(configuration)
            .border(Color.red)
    }
}
```

