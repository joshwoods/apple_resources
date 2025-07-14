

- Dispatch
- DispatchObject
-  suspend() 

Instance Method

# suspend()

Suspends the invocation of block objects on a dispatch object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func suspend()
```

## Discussion

By suspending a dispatch object, your application can temporarily prevent the execution of any blocks associated with that object. The suspension occurs after completion of any blocks running at the time of the call. Calling this function increments the suspension count of the object, and calling resume() decrements it. While the count is greater than zero, the object remains suspended, so you must balance each suspend() call with a matching resume() call.

Any blocks submitted to a dispatch queue or events observed by a dispatch source are delivered once the object is resumed.

Important

It is a programmer error to release an object that is currently suspended, because suspension implies that there is still work to be done. Therefore, always balance calls to this method with a corresponding call to resume() before disposing of the object. The behavior when releasing the last reference to a dispatch object while it is in a suspended state is undefined.

## See Also

### Activating, Suspending, and Resuming

func activate()

Activates the dispatch object.

func resume()

Resumes the invocation of block objects on a dispatch object.

