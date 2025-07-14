

- SwiftUI
- MenuStyle
-  MenuStyle.Configuration 

Type Alias

# MenuStyle.Configuration

The properties of a menu.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
typealias Configuration = MenuStyleConfiguration
```

## See Also

### Creating custom menu styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a menu.

**Required**

associatedtype Body : View

A view that represents the body of a menu.

**Required**

