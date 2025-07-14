

- SwiftUI
- ControlGroupStyle
-  Body 

Associated Type

# Body

A view representing the body of a control group.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
associatedtype Body : View
```

**Required**

## See Also

### Creating custom control group styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view representing the body of a control group.

**Required**

typealias Configuration

The properties of a `ControlGroup` instance being created.

