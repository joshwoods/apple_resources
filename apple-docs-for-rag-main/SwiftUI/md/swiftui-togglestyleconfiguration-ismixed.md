

- SwiftUI
- ToggleStyleConfiguration
-  isMixed 

Instance Property

# isMixed

Whether the Toggle is currently in a mixed state.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var isMixed: Bool
```

## Discussion

Use this property to determine whether the toggle style should render a mixed state presentation. A mixed state corresponds to an underlying collection with a mix of true and false Bindings. To toggle the state, use the `Bool.toggle()` method on the isOn binding.

In the following example, a custom style uses the `isMixed` property to render the correct toggle state using symbols:

```
struct SymbolToggleStyle: ToggleStyle {
    func makeBody(configuration: Configuration) -> some View {
        Button {
            configuration.isOn.toggle()
        } label: {
            Image(
                systemName: configuration.isMixed
                ? "minus.circle.fill" : configuration.isOn
                ? "checkmark.circle.fill" : "circle.fill")
            configuration.label
        }
    }
}
```

## See Also

### Managing the toggle state

var isOn: Bool

A binding to a state property that indicates whether the toggle is on.

var $isOn: Binding&lt;Bool>

