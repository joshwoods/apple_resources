

- Swift
- ThrowingTaskGroup
-  isCancelled 

Instance Property

# isCancelled

A Boolean value that indicates whether the group was canceled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isCancelled: Bool { get }
```

## Discussion

To cancel a group, call the `ThrowingTaskGroup.cancelAll()` method.

If the task that’s currently running this group is canceled, the group is also implicitly canceled, which is also reflected in this property’s value.

## See Also

### Canceling Tasks

func cancelAll()

Cancel all of the remaining tasks in the group.

