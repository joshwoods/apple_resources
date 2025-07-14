

- SwiftUI
- LayoutProperties
-  init() 

Initializer

# init()

Creates a default set of properties.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init()
```

## Discussion

Use a layout properties instance to provide information about a type that conforms to the Layout protocol. For example, you can create a layout properties instance in your layout’s implementation of the layoutProperties method, and use it to indicate that the layout has a Axis.vertical orientation:

```
extension BasicVStack {
    static var layoutProperties: LayoutProperties {
        var properties = LayoutProperties()
        properties.stackOrientation = .vertical
        return properties
    }
}
```

