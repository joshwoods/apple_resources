

- Dispatch
- DispatchObject
-  activate() 

Instance Method

# activate()

Activates the dispatch object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func activate()
```

## Discussion

Once a dispatch object has been activated, it cannot change its target queue.

## See Also

### Activating, Suspending, and Resuming

func resume()

Resumes the invocation of block objects on a dispatch object.

func suspend()

Suspends the invocation of block objects on a dispatch object.

