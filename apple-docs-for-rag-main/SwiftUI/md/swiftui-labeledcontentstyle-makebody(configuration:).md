

- SwiftUI
- LabeledContentStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of labeled content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## See Also

### Creating custom labeled content styles

typealias Configuration

The properties of a labeled content instance.

associatedtype Body : View

A view that represents the appearance and behavior of labeled content.

**Required**

