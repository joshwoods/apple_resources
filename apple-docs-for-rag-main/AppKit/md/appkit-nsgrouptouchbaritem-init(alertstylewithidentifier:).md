

- AppKit
- NSGroupTouchBarItem
-  init(alertStyleWithIdentifier:) 

Initializer

# init(alertStyleWithIdentifier:)

Initializes and returns a group item configured to match system alerts.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.13+

``` source
@MainActor
convenience init(alertStyleWithIdentifier identifier: NSTouchBarItem.Identifier)
```

## Discussion

You can control spacing between items, but it is recommended to use fixedSpaceLarge to maintain consistency.

The groupUserInterfaceLayoutDirection is set to match the application’s userInterfaceLayoutDirection.

## See Also

### Creating a group

convenience init(identifier: NSTouchBarItem.Identifier, items: [NSTouchBarItem])

Initializes and returns a group item whose bar is constructed from the supplied items.

convenience init(identifier: NSTouchBarItem.Identifier, items: [NSTouchBarItem], allowedCompressionOptions: NSUserInterfaceCompressionOptions)

Initializes and returns a group item whose bar is constructed from the supplied items, and with the specified compression options.

