

- SwiftUI
- ControlGroup
-  init(\_:) 

Initializer

# init(\_:)

Creates a control group based on a style configuration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(_ configuration: ControlGroupStyleConfiguration)
```

Available when `Content` is `ControlGroupStyleConfiguration.Content`.

## Discussion

Use this initializer within the makeBody(configuration:) method of a ControlGroupStyle instance to create an instance of the control group being styled. This is useful for custom control group styles that modify the current control group style.

For example, the following code creates a new, custom style that places a red border around the current control group:

```
struct RedBorderControlGroupStyle: ControlGroupStyle {
    func makeBody(configuration: Configuration) -> some View {
        ControlGroup(configuration)
            .border(Color.red)
    }
}
```

