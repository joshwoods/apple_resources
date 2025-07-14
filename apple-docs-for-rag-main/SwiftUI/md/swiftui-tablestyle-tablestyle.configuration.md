

- SwiftUI
- TableStyle
-  TableStyle.Configuration 

Type Alias

# TableStyle.Configuration

The properties of a table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
typealias Configuration = TableStyleConfiguration
```

## See Also

### Creating custom table styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a table.

**Required**

associatedtype Body : View

A view that represents the body of a table.

**Required**

