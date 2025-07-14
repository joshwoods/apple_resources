

- SwiftUI
- ToggleStyle
-  Body 

Associated Type

# Body

A view that represents the appearance and interaction of a toggle.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
associatedtype Body : View
```

**Required**

## Discussion

SwiftUI infers this type automatically based on the View instance that you return from your implementation of the makeBody(configuration:) method.

## See Also

### Creating custom toggle styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a toggle.

**Required**

struct ToggleStyleConfiguration

The properties of a toggle instance.

typealias Configuration

The properties of a toggle instance.

