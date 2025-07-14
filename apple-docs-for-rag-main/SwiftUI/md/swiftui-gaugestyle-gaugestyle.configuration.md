

- SwiftUI
- GaugeStyle
-  GaugeStyle.Configuration 

Type Alias

# GaugeStyle.Configuration

The properties of a gauge instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
typealias Configuration = GaugeStyleConfiguration
```

## See Also

### Creating custom gauge styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view representing the body of a gauge.

**Required**

associatedtype Body : View

A view representing the body of a gauge.

**Required**

