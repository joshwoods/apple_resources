

- SwiftUI
- LabelStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the label.

## Discussion

The system calls this method for each Label instance in a view hierarchy where this style is the current label style.

## See Also

### Creating custom label styles

typealias Configuration

The properties of a label.

associatedtype Body : View

A view that represents the body of a label.

**Required**

