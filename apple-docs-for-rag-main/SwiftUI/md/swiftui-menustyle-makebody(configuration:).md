

- SwiftUI
- MenuStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a menu.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the menu.

## Discussion

The system calls this method for each Menu instance in a view hierarchy where this style is the current menu style.

## See Also

### Creating custom menu styles

typealias Configuration

The properties of a menu.

associatedtype Body : View

A view that represents the body of a menu.

**Required**

