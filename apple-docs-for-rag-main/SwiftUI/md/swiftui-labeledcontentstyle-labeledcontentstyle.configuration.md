

- SwiftUI
- LabeledContentStyle
-  LabeledContentStyle.Configuration 

Type Alias

# LabeledContentStyle.Configuration

The properties of a labeled content instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias Configuration = LabeledContentStyleConfiguration
```

## See Also

### Creating custom labeled content styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of labeled content.

**Required**

associatedtype Body : View

A view that represents the appearance and behavior of labeled content.

**Required**

