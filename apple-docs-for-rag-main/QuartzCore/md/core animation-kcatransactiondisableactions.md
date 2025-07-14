

- Core Animation
-  kCATransactionDisableActions 

Global Variable

# kCATransactionDisableActions

A key whose value indicates whether implicit actions for property changes made within the transaction group are suppressed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
let kCATransactionDisableActions: String
```

## Discussion

If true, implicit actions for property changes made within the transaction group are suppressed. The value for this key must be an instance of NSNumber.

## See Also

### Constants

let kCATransactionAnimationDuration: String

Duration, in seconds, for animations triggered within the transaction group.

let kCATransactionAnimationTimingFunction: String

let kCATransactionCompletionBlock: String

