

- SwiftUI
- Widget
-  body 

Instance Property

# body

The content and behavior of the widget.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
var body: Self.Body { get }
```

**Required**

## Discussion

For any widgets that you create, provide a computed `body` property that defines the widget as a composition of SwiftUI views.

Swift infers the widget’s Body associated type based on the contents of the `body` property.

## See Also

### Implementing a widget

associatedtype Body : WidgetConfiguration

The type of configuration representing the content of the widget.

**Required**

