

- AppKit
- NSStepperTouchBarItem
-  init(identifier:drawingHandler:) 

Initializer

# init(identifier:drawingHandler:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
convenience init(
    identifier: NSTouchBarItem.Identifier,
    drawingHandler: @escaping (NSRect, Double) -> Void
)
```

## See Also

### Creating a stepper item

convenience init(identifier: NSTouchBarItem.Identifier, formatter: Formatter)

