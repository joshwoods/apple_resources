

- SwiftUI
- ToggleStyleConfiguration
-  label 

Instance Property

# label

A view that describes the effect of switching the toggle between states.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let label: ToggleStyleConfiguration.Label
```

## Discussion

Use this value in your implementation of the makeBody(configuration:) method when defining a custom ToggleStyle. Access it through the that method’s `configuration` parameter.

Because the label is a View, you can incorporate it into the view hierarchy that you return from your style definition. For example, you can combine the label with a circle image in an HStack:

```
HStack {
    Image(systemName: configuration.isOn
        ? "checkmark.circle.fill"
        : "circle")
    configuration.label
}
```

## See Also

### Getting the label view

struct Label

A type-erased label of a toggle.

