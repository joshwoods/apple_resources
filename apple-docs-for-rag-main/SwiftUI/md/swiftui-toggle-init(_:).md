

- SwiftUI
- Toggle
-  init(\_:) 

Initializer

# init(\_:)

Creates a toggle based on a toggle style configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(_ configuration: ToggleStyleConfiguration)
```

Available when `Label` is `ToggleStyleConfiguration.Label`.

## Parameters 

`configuration`  

The properties of the toggle, including a label and a binding to the toggle’s state.

## Discussion

You can use this initializer within the makeBody(configuration:) method of a ToggleStyle to create an instance of the styled toggle. This is useful for custom toggle styles that only modify the current toggle style, as opposed to implementing a brand new style.

For example, the following style adds a red border around the toggle, but otherwise preserves the toggle’s current style:

```
struct RedBorderToggleStyle: ToggleStyle {
    func makeBody(configuration: Configuration) -> some View {
        Toggle(configuration)
            .padding()
            .border(.red)
    }
}
```

