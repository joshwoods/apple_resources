

- SwiftUI
- ButtonStyle
-  ButtonStyle.Configuration 

Type Alias

# ButtonStyle.Configuration

The properties of a button.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Configuration = ButtonStyleConfiguration
```

## See Also

### Custom button styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a button.

**Required**

associatedtype Body : View

A view that represents the body of a button.

**Required**

