

- SwiftUI
- ControlGroupStyle
-  ControlGroupStyle.Configuration 

Type Alias

# ControlGroupStyle.Configuration

The properties of a `ControlGroup` instance being created.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
typealias Configuration = ControlGroupStyleConfiguration
```

## See Also

### Creating custom control group styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view representing the body of a control group.

**Required**

associatedtype Body : View

A view representing the body of a control group.

**Required**

