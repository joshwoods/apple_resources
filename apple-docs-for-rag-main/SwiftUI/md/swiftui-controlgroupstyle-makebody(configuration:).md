

- SwiftUI
- ControlGroupStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view representing the body of a control group.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the control group instance being created.

## Discussion

This method will be called for each instance of ControlGroup created within a view hierarchy where this style is the current `ControlGroupStyle`.

## See Also

### Creating custom control group styles

typealias Configuration

The properties of a `ControlGroup` instance being created.

associatedtype Body : View

A view representing the body of a control group.

**Required**

