

- SwiftUI
- ToggleStyle
-  ToggleStyle.Configuration 

Type Alias

# ToggleStyle.Configuration

The properties of a toggle instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Configuration = ToggleStyleConfiguration
```

## Discussion

You receive a `configuration` parameter of this type — which is an alias for the ToggleStyleConfiguration type — when you implement the required makeBody(configuration:) method in a custom toggle style implementation.

## See Also

### Creating custom toggle styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a toggle.

**Required**

struct ToggleStyleConfiguration

The properties of a toggle instance.

associatedtype Body : View

A view that represents the appearance and interaction of a toggle.

**Required**

