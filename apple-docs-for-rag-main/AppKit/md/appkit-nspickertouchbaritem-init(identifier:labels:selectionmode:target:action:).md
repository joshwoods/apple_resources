

- AppKit
- NSPickerTouchBarItem
-  init(identifier:labels:selectionMode:target:action:) 

Initializer

# init(identifier:labels:selectionMode:target:action:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
convenience init(
    identifier: NSTouchBarItem.Identifier,
    labels: [String],
    selectionMode: NSPickerTouchBarItem.SelectionMode,
    target: Any?,
    action: Selector?
)
```

## See Also

### Creating a picker item

convenience init(identifier: NSTouchBarItem.Identifier, images: [UIImage], selectionMode: NSPickerTouchBarItem.SelectionMode, target: Any?, action: Selector?)

