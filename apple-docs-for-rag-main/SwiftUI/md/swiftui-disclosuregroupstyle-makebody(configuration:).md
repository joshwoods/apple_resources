

- SwiftUI
- DisclosureGroupStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a disclosure group.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the instance being created.

## Discussion

SwiftUI calls this method for each instance of DisclosureGroup that you create within a view hierarchy where this style is the current DisclosureGroupStyle.

## See Also

### Creating custom disclosure group styles

struct DisclosureGroupStyleConfiguration

The properties of a disclosure group instance.

typealias Configuration

The properties of a disclosure group instance.

associatedtype Body : View

A view that represents the body of a disclosure group.

**Required**

