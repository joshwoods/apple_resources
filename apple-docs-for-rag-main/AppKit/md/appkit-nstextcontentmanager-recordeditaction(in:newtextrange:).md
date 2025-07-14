

- AppKit
- NSTextContentManager
-  recordEditAction(in:newTextRange:) 

Instance Method

# recordEditAction(in:newTextRange:)

Records information about an edit action to the transaction.

macOS 12.0+

``` source
func recordEditAction(
    in originalTextRange: NSTextRange,
    newTextRange: NSTextRange
)
```

## Parameters 

`originalTextRange`  

The range before the action.

`newTextRange`  

The corresponding range after the action.

## Discussion

The concrete subclass invokes this method for each edit action.

## See Also

### Performing transactions

var hasEditingTransaction: Bool

Indicates there’s an active editing transaction from the primary text layout manager.

func performEditingTransaction(() -> Void)

Performs an editing transaction and invokes a block upon completion.

