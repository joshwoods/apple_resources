

- AppKit
- NSResponder
-  restoreState(with:) 

Instance Method

# restoreState(with:)

Restores the interface-related state of the responder.

macOS 10.7+

``` source
@MainActor
func restoreState(with coder: NSCoder)
```

## Parameters 

`coder`  

The coder object to use to restore the responder’s interface-related state.

## Discussion

This method is part of the window restoration system and is called at launch time to restore the visual state of your responder object. The default implementation does nothing but specific subclasses (such as NSView and NSWindow) override it and save important state information. Therefore, if you override this method, you should always call `super` at some point in your implementation.

Subclasses can override this method and use it to restore any information that was saved in the encodeRestorableState(with:) method. You can also use this method to reconfigure the responder to its previous appearance.

Note

If the user’s computer is configured to close all windows when an app quits, the system automatically removes any preserved state as part of that process. As a result, the system doesn’t call `restoreState(with:)` the next time your app launches.

For information about using a coder object to read data from an archive, see Encoding and Decoding Custom Types.

## See Also

### Handling Window Restoration

class func allowedClasses(forRestorableStateKeyPath: String) -> [AnyClass]

Returns the classes that support secure coding.

func encodeRestorableState(with: NSCoder)

Saves the interface-related state of the responder.

func encodeRestorableState(with: NSCoder, backgroundQueue: OperationQueue)

Saves the interface-related state of the responder to a keyed archiver either synchronously or asynchronously on the given operation queue.

class var restorableStateKeyPaths: [String]

Returns an array of key paths representing the restorable attributes of the responder.

func invalidateRestorableState()

Marks the responder’s interface-related state as dirty.

