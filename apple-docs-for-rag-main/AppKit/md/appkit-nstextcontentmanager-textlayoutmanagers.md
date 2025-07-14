

- AppKit
- NSTextContentManager
-  textLayoutManagers 

Instance Property

# textLayoutManagers

The array of text layout managers associated with this text content manager.

macOS 12.0+

``` source
var textLayoutManagers: [NSTextLayoutManager] { get }
```

## Discussion

This property is KVO-compliant.

## See Also

### Working with layout managers

var primaryTextLayoutManager: NSTextLayoutManager?

The primary text layout manager for this content.

var automaticallySynchronizesTextLayoutManagers: Bool

Determines if the framework should automatically synchronize all text layout managers when exiting an editing transaction.

func addTextLayoutManager(NSTextLayoutManager)

Adds the layout manager you provide to the list of layout managers.

func removeTextLayoutManager(NSTextLayoutManager)

Removes the layout manager you specifiy from the list of layout managers.

func synchronizeTextLayoutManagers((((any Error)?) -> Void)?)

Synchronizes changes to all nonprimary text layout managers.

