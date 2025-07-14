

- Swift Charts
-  Plot 

Structure

# Plot

A mechanism for grouping chart contents into a single entity.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct Plot where Content : ChartContent
```

## Topics

### Initializers

init(content: () -> Content)

## Relationships

### Conforms To

- ChartContent

  Conforms when `Content` conforms to `ChartContent`.

- Copyable
- Sendable

## See Also

### Charts

Creating a chart using Swift Charts

Make a chart by combining chart building blocks in SwiftUI.

Visualizing your app’s data

Build complex and interactive charts using Swift Charts.

struct Chart

A SwiftUI view that displays a chart.

protocol ChartContent

A type that represents the content that you draw on a chart.

struct ChartContentBuilder

A result builder that you use to compose the contents of a chart.

