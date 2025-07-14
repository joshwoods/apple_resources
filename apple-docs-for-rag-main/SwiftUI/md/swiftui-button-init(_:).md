

- SwiftUI
- Button
-  init(\_:) 

Initializer

# init(\_:)

Creates a button based on a configuration for a style with a custom appearance and custom interaction behavior.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(_ configuration: PrimitiveButtonStyleConfiguration)
```

Available when `Label` is `PrimitiveButtonStyleConfiguration.Label`.

## Parameters 

`configuration`  

A configuration for a style with a custom appearance and custom interaction behavior.

## Discussion

Use this initializer within the makeBody(configuration:) method of a PrimitiveButtonStyle to create an instance of the button that you want to style. This is useful for custom button styles that modify the current button style, rather than implementing a brand new style.

For example, the following style adds a red border around the button, but otherwise preserves the button’s current style:

```
struct RedBorderedButtonStyle: PrimitiveButtonStyle {
    func makeBody(configuration: Configuration) -> some View {
        Button(configuration)
            .border(Color.red)
    }
}
```

