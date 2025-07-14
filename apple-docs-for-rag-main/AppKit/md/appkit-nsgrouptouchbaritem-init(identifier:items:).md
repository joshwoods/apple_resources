

- AppKit
- NSGroupTouchBarItem
-  init(identifier:items:) 

Initializer

# init(identifier:items:)

Initializes and returns a group item whose bar is constructed from the supplied items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
convenience init(
    identifier: NSTouchBarItem.Identifier,
    items: [NSTouchBarItem]
)
```

## See Also

### Creating a group

convenience init(identifier: NSTouchBarItem.Identifier, items: [NSTouchBarItem], allowedCompressionOptions: NSUserInterfaceCompressionOptions)

Initializes and returns a group item whose bar is constructed from the supplied items, and with the specified compression options.

convenience init(alertStyleWithIdentifier: NSTouchBarItem.Identifier)

Initializes and returns a group item configured to match system alerts.

