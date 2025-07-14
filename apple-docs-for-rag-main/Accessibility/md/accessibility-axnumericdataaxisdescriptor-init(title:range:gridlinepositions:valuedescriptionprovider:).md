

- Accessibility
- AXNumericDataAxisDescriptor
-  init(title:range:gridlinePositions:valueDescriptionProvider:) 

Initializer

# init(title:range:gridlinePositions:valueDescriptionProvider:)

Creates a numeric data axis with the specified title, range, gridline positions, and value description provider closure.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
convenience init(
    title: String,
    range: ClosedRange,
    gridlinePositions: [Double],
    valueDescriptionProvider: @escaping (Double) -> String
)
```

## See Also

### Creating a numeric data axis

convenience init(attributedTitle: NSAttributedString, range: ClosedRange&lt;Double>, gridlinePositions: [Double], valueDescriptionProvider: (Double) -> String)

Creates a numeric data axis with the specified attributed title, range, gridline positions, and value description provider closure.

