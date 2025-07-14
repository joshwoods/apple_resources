

- AppKit
- NSTextContentManager
-  primaryTextLayoutManager 

Instance Property

# primaryTextLayoutManager

The primary text layout manager for this content.

macOS 12.0+

``` source
var primaryTextLayoutManager: NSTextLayoutManager? { get set }
```

## Discussion

Setting this property to an NSTextLayoutManager not in `textLayoutManagers` resets it to `nil`. It automatically synchronizes pending edits before switching to a new primary object. The operation is synchronous.

This property is KVO-compliant.

## See Also

### Working with layout managers

var textLayoutManagers: [NSTextLayoutManager]

The array of text layout managers associated with this text content manager.

var automaticallySynchronizesTextLayoutManagers: Bool

Determines if the framework should automatically synchronize all text layout managers when exiting an editing transaction.

func addTextLayoutManager(NSTextLayoutManager)

Adds the layout manager you provide to the list of layout managers.

func removeTextLayoutManager(NSTextLayoutManager)

Removes the layout manager you specifiy from the list of layout managers.

func synchronizeTextLayoutManagers((((any Error)?) -> Void)?)

Synchronizes changes to all nonprimary text layout managers.

