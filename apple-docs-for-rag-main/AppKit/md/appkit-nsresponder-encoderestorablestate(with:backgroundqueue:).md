

- AppKit
- NSResponder
-  encodeRestorableState(with:backgroundQueue:) 

Instance Method

# encodeRestorableState(with:backgroundQueue:)

Saves the interface-related state of the responder to a keyed archiver either synchronously or asynchronously on the given operation queue.

macOS 10.13+

``` source
@MainActor
func encodeRestorableState(
    with coder: NSCoder,
    backgroundQueue queue: OperationQueue
)
```

## Parameters 

`coder`  

A thread-safe keyed archiver to write restorable state into.

`queue`  

A serial background operation queue to perform asynchronous encoding work on.

## Discussion

Don’t call this method directly. The system calls this method on the main thread. The receiver may synchronously encode state to `coder` or may enqueue asynchronous work to encode additional restorable state using the provided serial background OperationQueue, if it can safely access and encode that information. The encoding process finishes when the enqueued operations complete.

If you override this method, call the super implementation.

## See Also

### Handling Window Restoration

class func allowedClasses(forRestorableStateKeyPath: String) -> [AnyClass]

Returns the classes that support secure coding.

func encodeRestorableState(with: NSCoder)

Saves the interface-related state of the responder.

func restoreState(with: NSCoder)

Restores the interface-related state of the responder.

class var restorableStateKeyPaths: [String]

Returns an array of key paths representing the restorable attributes of the responder.

func invalidateRestorableState()

Marks the responder’s interface-related state as dirty.

