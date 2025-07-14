

- AppKit
- NSTextContentManager
-  addTextLayoutManager(\_:) 

Instance Method

# addTextLayoutManager(\_:)

Adds the layout manager you provide to the list of layout managers.

macOS 12.0+

``` source
func addTextLayoutManager(_ textLayoutManager: NSTextLayoutManager)
```

## Parameters 

`textLayoutManager`  

The layout manager to add.

## See Also

### Working with layout managers

var primaryTextLayoutManager: NSTextLayoutManager?

The primary text layout manager for this content.

var textLayoutManagers: [NSTextLayoutManager]

The array of text layout managers associated with this text content manager.

var automaticallySynchronizesTextLayoutManagers: Bool

Determines if the framework should automatically synchronize all text layout managers when exiting an editing transaction.

func removeTextLayoutManager(NSTextLayoutManager)

Removes the layout manager you specifiy from the list of layout managers.

func synchronizeTextLayoutManagers((((any Error)?) -> Void)?)

Synchronizes changes to all nonprimary text layout managers.

