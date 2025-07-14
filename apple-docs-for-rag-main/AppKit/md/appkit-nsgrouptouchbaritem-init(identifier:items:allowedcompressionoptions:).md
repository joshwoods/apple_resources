

- AppKit
- NSGroupTouchBarItem
-  init(identifier:items:allowedCompressionOptions:) 

Initializer

# init(identifier:items:allowedCompressionOptions:)

Initializes and returns a group item whose bar is constructed from the supplied items, and with the specified compression options.

macOS 10.13+

``` source
@MainActor
convenience init(
    identifier: NSTouchBarItem.Identifier,
    items: [NSTouchBarItem],
    allowedCompressionOptions: NSUserInterfaceCompressionOptions
)
```

## Discussion

Use this initializer to specify which compression options are applied to the group item. The system applies options in the following default order: `breakEqualWidths`, `reduceMetrics`, `hideText`, `hideImages`.

If you want to use non-standard compression options, add them by using the prioritizedCompressionOptions property.

## See Also

### Creating a group

convenience init(identifier: NSTouchBarItem.Identifier, items: [NSTouchBarItem])

Initializes and returns a group item whose bar is constructed from the supplied items.

convenience init(alertStyleWithIdentifier: NSTouchBarItem.Identifier)

Initializes and returns a group item configured to match system alerts.

