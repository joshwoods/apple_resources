

- Dispatch
- DispatchWorkItem
-  isCancelled 

Instance Property

# isCancelled

A Boolean value indicating whether the work item has been canceled.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
var isCancelled: Bool { get }
```

## Discussion

The value of this property is true if the work item has been canceled.

## See Also

### Canceling a Work Item

func cancel()

Cancels the current work item asynchronously.

