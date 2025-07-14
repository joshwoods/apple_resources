

- AppKit
- NSTextStorageObserving
-  performEditingTransaction(for:using:) 

Instance Method

# performEditingTransaction(for:using:)

macOS 12.0+

``` source
func performEditingTransaction(
    for textStorage: NSTextStorage,
    using transaction: () -> Void
)
```

**Required**

## See Also

### Managing the editing process

func processEditing(for: NSTextStorage, edited: NSTextStorageEditActions, range: NSRange, changeInLength: Int, invalidatedRange: NSRange)

**Required**

