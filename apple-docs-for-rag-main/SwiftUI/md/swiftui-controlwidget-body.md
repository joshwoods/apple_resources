

- SwiftUI
- ControlWidget
-  body 

Instance Property

# body

The content and behavior of the control.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@ControlWidgetConfigurationBuilder @MainActor @preconcurrency
var body: Self.Body { get }
```

**Required**

## Discussion

For any controls that you create, provide a computed `body` property that defines the control using some control widget configuration.

Swift infers the control’s Body associated type based on the contents of the `body` property.

