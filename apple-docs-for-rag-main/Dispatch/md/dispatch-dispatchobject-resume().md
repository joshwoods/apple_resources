

- Dispatch
- DispatchObject
-  resume() 

Instance Method

# resume()

Resumes the invocation of block objects on a dispatch object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func resume()
```

## Discussion

Calling this function decrements the suspension count of a suspended dispatch queue or dispatch event source object. While the count is greater than zero, the object remains suspended. When the suspension count returns to zero, any blocks submitted to the dispatch queue or any events observed by the dispatch source while suspended are delivered.

With one exception, each call to resume() must balance a call to suspend(). New dispatch event source objects returned by dispatch_source_create have a suspension count of 1 and must be resumed before any events are delivered. This approach allows your application to fully configure the dispatch event source object prior to delivery of the first event. In all other cases, it is undefined to call resume() more times than suspend(), which would result in a negative suspension count.

## See Also

### Activating, Suspending, and Resuming

func activate()

Activates the dispatch object.

func suspend()

Suspends the invocation of block objects on a dispatch object.

