

- CallKit
- CXCallObserver
-  setDelegate(\_:queue:) 

Instance Method

# setDelegate(\_:queue:)

Sets a call observer delegate, specifying an optional queue on which to execute delegate methods.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func setDelegate(
    _ delegate: (any CXCallObserverDelegate)?,
    queue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

An object conforming to the `CXCallObserverDelegate` protocol.

`queue`  

The queue on which to execute delegate methods.

If `nil`, delegate methods are performed on the main queue.

Important

Any queue specified is stored as a weak reference.

