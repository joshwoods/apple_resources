

- AppKit
- NSResponder
-  allowedClasses(forRestorableStateKeyPath:) 

Type Method

# allowedClasses(forRestorableStateKeyPath:)

Returns the classes that support secure coding.

macOS 12.0+

``` source
@MainActor
class func allowedClasses(forRestorableStateKeyPath keyPath: String) -> [AnyClass]
```

## Parameters 

`keyPath`  

The key path of the restorable object.

## Return Value

An array of classes that support secure coding.

## Discussion

The system calls the function during a secure state restoration and restores values only for the allowed classes your app returns in the array.

## See Also

### Handling Window Restoration

func encodeRestorableState(with: NSCoder)

Saves the interface-related state of the responder.

func encodeRestorableState(with: NSCoder, backgroundQueue: OperationQueue)

Saves the interface-related state of the responder to a keyed archiver either synchronously or asynchronously on the given operation queue.

func restoreState(with: NSCoder)

Restores the interface-related state of the responder.

class var restorableStateKeyPaths: [String]

Returns an array of key paths representing the restorable attributes of the responder.

func invalidateRestorableState()

Marks the responder’s interface-related state as dirty.

