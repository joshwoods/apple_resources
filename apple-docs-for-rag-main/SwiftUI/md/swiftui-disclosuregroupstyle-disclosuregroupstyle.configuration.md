

- SwiftUI
- DisclosureGroupStyle
-  DisclosureGroupStyle.Configuration 

Type Alias

# DisclosureGroupStyle.Configuration

The properties of a disclosure group instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
typealias Configuration = DisclosureGroupStyleConfiguration
```

## See Also

### Creating custom disclosure group styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a disclosure group.

**Required**

struct DisclosureGroupStyleConfiguration

The properties of a disclosure group instance.

associatedtype Body : View

A view that represents the body of a disclosure group.

**Required**

