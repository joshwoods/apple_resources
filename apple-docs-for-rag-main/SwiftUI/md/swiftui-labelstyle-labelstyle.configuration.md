

- SwiftUI
- LabelStyle
-  LabelStyle.Configuration 

Type Alias

# LabelStyle.Configuration

The properties of a label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
typealias Configuration = LabelStyleConfiguration
```

## See Also

### Creating custom label styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a label.

**Required**

associatedtype Body : View

A view that represents the body of a label.

**Required**

