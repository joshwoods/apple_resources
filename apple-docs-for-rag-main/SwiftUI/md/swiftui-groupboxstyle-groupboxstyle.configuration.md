

- SwiftUI
- GroupBoxStyle
-  GroupBoxStyle.Configuration 

Type Alias

# GroupBoxStyle.Configuration

The properties of a group box instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
typealias Configuration = GroupBoxStyleConfiguration
```

## See Also

### Creating custom group box styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view representing the body of a group box.

**Required**

associatedtype Body : View

A view that represents the body of a group box.

**Required**

