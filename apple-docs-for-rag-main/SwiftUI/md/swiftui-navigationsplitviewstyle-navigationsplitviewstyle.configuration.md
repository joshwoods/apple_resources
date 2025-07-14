

- SwiftUI
- NavigationSplitViewStyle
-  NavigationSplitViewStyle.Configuration 

Type Alias

# NavigationSplitViewStyle.Configuration

The properties of a navigation split view instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias Configuration = NavigationSplitViewStyleConfiguration
```

## See Also

### Creating custom styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a navigation split view.

**Required**

associatedtype Body : View

A view that represents the body of a navigation split view.

**Required**

