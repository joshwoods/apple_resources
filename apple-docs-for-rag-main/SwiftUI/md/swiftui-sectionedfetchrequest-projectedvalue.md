

- SwiftUI
- SectionedFetchRequest
-  projectedValue 

Instance Property

# projectedValue

A binding to the request’s mutable configuration properties.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
var projectedValue: Binding.Configuration> { get }
```

## Discussion

This property behaves like the projectedValue of a FetchRequest. In particular, SwiftUI returns the value associated with this property when you use SectionedFetchRequest as a property wrapper on a SectionedFetchResults instance and then access the results with a dollar sign (`$`) prefix. The value that SwiftUI returns is a Binding to the request’s SectionedFetchRequest.Configuration structure, which dynamically configures the request.

## See Also

### Configuring a request dynamically

struct Configuration

The request’s configurable properties.

