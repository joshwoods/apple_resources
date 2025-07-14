

- Dispatch
- DispatchGroup
-  leave() 

Instance Method

# leave()

Explicitly indicates that a block in the group finished executing.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func leave()
```

## Discussion

Calling this function decrements the current count of outstanding tasks in the group. Using this function (with enter()) allows your application to properly manage the task reference count if it explicitly adds and removes tasks from the group by a means other than using the dispatch_group_async function.

A call to this function must balance a call to enter(). It is invalid to call it more times than enter(), which would result in a negative count.

## See Also

### Updating the Group Manually

func enter()

Explicitly indicates that a block has entered the group.

