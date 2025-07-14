

- Matter
- MTRDevice
-  wait(forAttributeValues:timeout:queue:completion:) 

Instance Method

# wait(forAttributeValues:timeout:queue:completion:)

Sets up the provided completion to be called when any of the following happens:

iOS 18.3+iPadOS 18.3+Mac Catalyst 18.3+macOS 15.3+tvOS 18.3+visionOS 2.3+watchOS 11.3+

``` source
func wait(
    forAttributeValues values: [MTRAttributePath : [String : Any]],
    timeout: TimeInterval,
    queue: dispatch_queue_t,
    completion: @escaping ((any Error)?) -> Void
) -> MTRAttributeValueWaiter
```

## Discussion

1.  A set of attributes reaches certain values: completion called with nil.

2.  The provided timeout expires: completion called with MTRErrorCodeTimeout error.

3.  The wait is canceled: completion called with MTRErrorCodeCancelled error.

If the MTRAttributeValueWaiter is destroyed before the completion is called, that is treated the same as canceling the waiter.

The attributes and values to wait for are represented as a dictionary which has the attribute paths as keys and the expected data-values as values.

