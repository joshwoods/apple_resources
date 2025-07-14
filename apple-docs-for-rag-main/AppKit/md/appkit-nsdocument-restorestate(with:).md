

- AppKit
- NSDocument
-  restoreState(with:) 

Instance Method

# restoreState(with:)

Restores the interface-related state of the document.

macOS 10.7+

``` source
@MainActor
func restoreState(with coder: NSCoder)
```

## Parameters 

`coder`  

The coder object to use to restore the document’s interface-related state.

## Discussion

This method is part of the window restoration system and is called at launch time to restore the window-related state of your document object. The default implementation restores some basic information about the document. If you override this method, you must call `super` at some point in your implementation.

Subclasses can override this method and use it to restore the document-related information that was saved in the encodeRestorableState(with:) method. You can also use this method to reconfigure the document (or its associated window controller and window) to their previous appearance.

Note

If the user’s computer is configured to close all windows when an app quits, the system automatically removes any preserved state as part of that process. As a result, the system doesn’t call `restoreState(with:)` the next time your app launches.

For information about using a coder object to read data from an archive, see Encoding and Decoding Custom Types.

## See Also

### Handling Window Restoration

class func allowedClasses(forRestorableStateKeyPath: String) -> [AnyClass]

Returns the classes that support secure coding.

func encodeRestorableState(with: NSCoder)

Saves the interface-related state of the document.

class var restorableStateKeyPaths: [String]

Returns an array of key paths that represent the restorable attributes of the document.

func invalidateRestorableState()

Marks the document’s interface-related state as dirty.

func restoreWindow(withIdentifier: NSUserInterfaceItemIdentifier, state: NSCoder, completionHandler: (NSWindow?, (any Error)?) -> Void)

Restores a window that was associated with a document, after that document is reopened.

