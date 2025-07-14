

- SwiftUI
- GroupBoxStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view representing the body of a group box.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the group box instance being created.

## Discussion

SwiftUI calls this method for each instance of GroupBox created within a view hierarchy where this style is the current group box style.

## See Also

### Creating custom group box styles

typealias Configuration

The properties of a group box instance.

associatedtype Body : View

A view that represents the body of a group box.

**Required**

