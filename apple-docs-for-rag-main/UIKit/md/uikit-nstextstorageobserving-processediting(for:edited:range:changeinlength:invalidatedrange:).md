

- UIKit
- NSTextStorageObserving
-  processEditing(for:edited:range:changeInLength:invalidatedRange:) 

Instance Method

# processEditing(for:edited:range:changeInLength:invalidatedRange:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func processEditing(
    for textStorage: NSTextStorage,
    edited editMask: NSTextStorage.EditActions,
    range newCharRange: NSRange,
    changeInLength delta: Int,
    invalidatedRange invalidatedCharRange: NSRange
)
```

**Required**

## See Also

### Managing the editing process

func performEditingTransaction(for: NSTextStorage, using: () -> Void)

**Required**

