

- AppKit
- NSDocument
-  invalidateRestorableState() 

Instance Method

# invalidateRestorableState()

Marks the document’s interface-related state as dirty.

macOS 10.7+

``` source
@MainActor
func invalidateRestorableState()
```

## Discussion

Call this method whenever the restorable state of your document changes. This method marks the document’s state as dirty, which causes that state to be written to disk at some point in the future. Do not override this method.

## See Also

### Handling Window Restoration

class func allowedClasses(forRestorableStateKeyPath: String) -> [AnyClass]

Returns the classes that support secure coding.

func encodeRestorableState(with: NSCoder)

Saves the interface-related state of the document.

func restoreState(with: NSCoder)

Restores the interface-related state of the document.

class var restorableStateKeyPaths: [String]

Returns an array of key paths that represent the restorable attributes of the document.

func restoreWindow(withIdentifier: NSUserInterfaceItemIdentifier, state: NSCoder, completionHandler: (NSWindow?, (any Error)?) -> Void)

Restores a window that was associated with a document, after that document is reopened.

