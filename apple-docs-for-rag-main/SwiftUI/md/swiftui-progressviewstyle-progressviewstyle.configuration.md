

- SwiftUI
- ProgressViewStyle
-  ProgressViewStyle.Configuration 

Type Alias

# ProgressViewStyle.Configuration

A type alias for the properties of a progress view instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
typealias Configuration = ProgressViewStyleConfiguration
```

## See Also

### Creating custom progress view styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view representing the body of a progress view.

**Required**

associatedtype Body : View

A view representing the body of a progress view.

**Required**

