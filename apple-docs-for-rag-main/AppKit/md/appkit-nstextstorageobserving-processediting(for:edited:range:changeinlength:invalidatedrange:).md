

- AppKit
- NSTextStorageObserving
-  processEditing(for:edited:range:changeInLength:invalidatedRange:) 

Instance Method

# processEditing(for:edited:range:changeInLength:invalidatedRange:)

macOS 12.0+

``` source
func processEditing(
    for textStorage: NSTextStorage,
    edited editMask: NSTextStorageEditActions,
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

