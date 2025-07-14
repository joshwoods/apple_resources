

- AppKit
- NSResponder
-  encodeRestorableState(with:) 

Instance Method

# encodeRestorableState(with:)

Saves the interface-related state of the responder.

macOS 10.7+

``` source
@MainActor
func encodeRestorableState(with coder: NSCoder)
```

## Parameters 

`coder`  

The coder object in which to save the responder’s interface-related state.

## Discussion

This method is part of the window restoration system and is called at appropriate times to save the visual state of your responder to the specified archive. The default implementation of this method does nothing but specific subclasses (such as NSView and NSWindow) override it to save important state information. Therefore, if you override this method, you should always call `super` at some point in your implementation.

Subclasses can override this method and use it to restore any information that would be needed to restore the responder to its current state. For example, the NSTabView class uses this method to save information about the currently selected tab. You must store enough data to reconfigure the responder and return it to its current state during a subsequent launch of the application.

For information about using a coder object to write data to an archive, see Archives and Serializations Programming Guide.

## See Also

### Handling Window Restoration

class func allowedClasses(forRestorableStateKeyPath: String) -> [AnyClass]

Returns the classes that support secure coding.

func encodeRestorableState(with: NSCoder, backgroundQueue: OperationQueue)

Saves the interface-related state of the responder to a keyed archiver either synchronously or asynchronously on the given operation queue.

func restoreState(with: NSCoder)

Restores the interface-related state of the responder.

class var restorableStateKeyPaths: [String]

Returns an array of key paths representing the restorable attributes of the responder.

func invalidateRestorableState()

Marks the responder’s interface-related state as dirty.

