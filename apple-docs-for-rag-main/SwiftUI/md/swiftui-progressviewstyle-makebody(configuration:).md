

- SwiftUI
- ProgressViewStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view representing the body of a progress view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the progress view being created.

## Discussion

The view hierarchy calls this method for each progress view where this style is the current progress view style.

## See Also

### Creating custom progress view styles

typealias Configuration

A type alias for the properties of a progress view instance.

associatedtype Body : View

A view representing the body of a progress view.

**Required**

