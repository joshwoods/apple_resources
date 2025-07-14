

- AppKit
- NSDocument
-  encodeRestorableState(with:) 

Instance Method

# encodeRestorableState(with:)

Saves the interface-related state of the document.

macOS 10.7+

``` source
@MainActor
func encodeRestorableState(with coder: NSCoder)
```

## Parameters 

`coder`  

The coder object in which to save the document’s interface-related state.

## Discussion

This method is part of the window restoration system and is called at appropriate times to save your document’s window-related state information to the specified archive. The default implementation of this method records some basic information about the document. If you override this method, you must call `super` at some point in your implementation.

Subclasses can override this method and use it to restore any information that would be needed to restore the document’s window to its current state. For example, you could use this method to record references to the data currently managed by the document and displayed by the window. (Do not store the actual data itself. Store only references to the data so that you can load it later from disk.) You must store enough data to reconfigure the document and its window to their current state during a subsequent launch of the app.

For information about using a coder object to write data to an archive, see Archives and Serializations Programming Guide.

## See Also

### Handling Window Restoration

class func allowedClasses(forRestorableStateKeyPath: String) -> [AnyClass]

Returns the classes that support secure coding.

func restoreState(with: NSCoder)

Restores the interface-related state of the document.

class var restorableStateKeyPaths: [String]

Returns an array of key paths that represent the restorable attributes of the document.

func invalidateRestorableState()

Marks the document’s interface-related state as dirty.

func restoreWindow(withIdentifier: NSUserInterfaceItemIdentifier, state: NSCoder, completionHandler: (NSWindow?, (any Error)?) -> Void)

Restores a window that was associated with a document, after that document is reopened.

