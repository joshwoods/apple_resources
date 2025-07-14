

- SwiftUI
- GaugeStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view representing the body of a gauge.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties to apply to the gauge instance.

## Discussion

The system calls this modifier on each instance of gauge within a view hierarchy where this style is the current gauge style.

## See Also

### Creating custom gauge styles

typealias Configuration

The properties of a gauge instance.

associatedtype Body : View

A view representing the body of a gauge.

**Required**

