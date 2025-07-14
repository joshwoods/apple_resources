

- SwiftUI
- LayoutProperties
-  stackOrientation 

Instance Property

# stackOrientation

The orientation of the containing stack-like container.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var stackOrientation: Axis?
```

## Discussion

Certain views alter their behavior based on the stack orientation of the container that they appear in. For example, Spacer and Divider align their major axis to match that of their container.

Set the orientation for your custom layout container by returning a configured LayoutProperties instance from your Layout type’s implementation of the layoutProperties method. For example, you can indicate that your layout has a Axis.vertical major axis:

```
extension BasicVStack {
    static var layoutProperties: LayoutProperties {
        var properties = LayoutProperties()
        properties.stackOrientation = .vertical
        return properties
    }
}
```

A value of `nil`, which is the default when you don’t specify a value, indicates an unknown orientation, or that a layout isn’t one-dimensional.

