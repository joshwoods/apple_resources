

- AppKit
- NSTextContentManager
-  performEditingTransaction(\_:) 

Instance Method

# performEditingTransaction(\_:)

Performs an editing transaction and invokes a block upon completion.

macOS 12.0+

``` source
func performEditingTransaction(_ transaction: () -> Void)
```

## Parameters 

`transaction`  

The editing transaction.

## Discussion

The primary NSTextLayoutManager controlling the active editing transaction invokes this method. It’s possible to nest multiple editing transactions. The outer most transaction toggles `hasEditingTransaction` and sends synchronization messages if enabled after invoking a transaction.

## See Also

### Performing transactions

var hasEditingTransaction: Bool

Indicates there’s an active editing transaction from the primary text layout manager.

func recordEditAction(in: NSTextRange, newTextRange: NSTextRange)

Records information about an edit action to the transaction.

