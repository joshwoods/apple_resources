

- SwiftUI
- NavigationSplitViewStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a navigation split view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the instance to create.

## Discussion

SwiftUI calls this method for each instance of NavigationSplitView, where this style is the current NavigationSplitViewStyle.

## See Also

### Creating custom styles

typealias Configuration

The properties of a navigation split view instance.

associatedtype Body : View

A view that represents the body of a navigation split view.

**Required**

