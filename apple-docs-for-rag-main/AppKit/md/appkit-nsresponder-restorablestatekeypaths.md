

- AppKit
- NSResponder
-  restorableStateKeyPaths 

Type Property

# restorableStateKeyPaths

Returns an array of key paths representing the restorable attributes of the responder.

macOS 10.7+

``` source
@MainActor
class var restorableStateKeyPaths: [String] { get }
```

## Return Value

An array of NSString objects, each of which contains a key path to one of the responder’s attributes.

## Discussion

You can use this method instead of, or in addition to, the encodeRestorableState(with:) and restoreState(with:) methods to save and restore the state of your responder. The key paths you return must refer to attributes that are key-value coding and key-value observing compliant. To learn more about these mechanisms, see Key-Value Coding Programming Guide and Key-Value Observing Programming Guide.

When changes are detected, the specified attributes are automatically written to disk with the rest of the application’s interface-related state. At launch time, the attributes are automatically restored to their previous values.

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

func invalidateRestorableState()

Marks the responder’s interface-related state as dirty.

