

- AppKit
- NSResponder
-  invalidateRestorableState() 

Instance Method

# invalidateRestorableState()

Marks the responder’s interface-related state as dirty.

macOS 10.7+

``` source
@MainActor
func invalidateRestorableState()
```

## Discussion

Call this method whenever the restorable state of your responder changes. This method marks the responder’s state as dirty, which writes the state to disk at some point in the future. Don’t override this method.

## See Also

### Handling Window Restoration

class func allowedClasses(forRestorableStateKeyPath: String) -> [AnyClass]

Returns the classes that support secure coding.

func encodeRestorableState(with: NSCoder)

Saves the interface-related state of the responder.

func encodeRestorableState(with: NSCoder, backgroundQueue: OperationQueue)

Saves the interface-related state of the responder to a keyed archiver either synchronously or asynchronously on the given operation queue.

func restoreState(with: NSCoder)

Restores the interface-related state of the responder.

class var restorableStateKeyPaths: [String]

Returns an array of key paths representing the restorable attributes of the responder.

