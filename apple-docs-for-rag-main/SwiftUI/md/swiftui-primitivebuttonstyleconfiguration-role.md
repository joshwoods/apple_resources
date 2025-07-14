

- SwiftUI
- PrimitiveButtonStyleConfiguration
-  role 

Instance Property

# role

An optional semantic role describing the button’s purpose.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let role: ButtonRole?
```

## Discussion

A value of `nil` means that the Button has no assigned role. If the button does have a role, use it to make adjustments to the button’s appearance. The following example shows a custom style that uses bold text when the role is cancel, red text when the role is destructive, and adds no special styling otherwise:

```
struct MyButtonStyle: PrimitiveButtonStyle {
    func makeBody(configuration: Configuration) -> some View {
        configuration.label
            .onTapGesture {
                configuration.trigger()
            }
            .font(
                configuration.role == .cancel ? .title2.bold() : .title2)
            .foregroundColor(
                configuration.role == .destructive ? Color.red : nil)
    }
}
```

You can create one of each button using this style to see the effect:

```
VStack(spacing: 20) {
    Button("Cancel", role: .cancel) {}
    Button("Delete", role: .destructive) {}
    Button("Continue") {}
}
.buttonStyle(MyButtonStyle())
```

