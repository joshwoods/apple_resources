

- SwiftUI
- TableStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the table.

## Discussion

The system calls this method for each Table instance in a view hierarchy where this style is the current table style.

## See Also

### Creating custom table styles

typealias Configuration

The properties of a table.

associatedtype Body : View

A view that represents the body of a table.

**Required**

