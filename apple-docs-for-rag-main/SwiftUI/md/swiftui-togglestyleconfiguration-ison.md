

- SwiftUI
- ToggleStyleConfiguration
-  isOn 

Instance Property

# isOn

A binding to a state property that indicates whether the toggle is on.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@Binding
var isOn: Bool { get nonmutating set }
```

## Discussion

Because this value is a Binding, you can both read and write it in your implementation of the makeBody(configuration:) method when defining a custom ToggleStyle. Access it through that method’s `configuration` parameter.

Read this value to set the appearance of the toggle. For example, you can choose between empty and filled circles based on the `isOn` value:

```
Image(systemName: configuration.isOn
    ? "checkmark.circle.fill"
    : "circle")
```

Write this value when the user takes an action that’s meant to change the state of the toggle. For example, you can toggle it inside the `action` closure of a Button instance:

```
Button {
    configuration.isOn.toggle()
} label: {
    // Draw the toggle.
}
```

## See Also

### Managing the toggle state

var isMixed: Bool

Whether the Toggle is currently in a mixed state.

var $isOn: Binding&lt;Bool>

