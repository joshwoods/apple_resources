

- AppKit
- NSDocument
-  restorableStateKeyPaths 

Type Property

# restorableStateKeyPaths

Returns an array of key paths that represent the restorable attributes of the document.

macOS 10.7+

``` source
@MainActor
class var restorableStateKeyPaths: [String] { get }
```

## Return Value

An array of NSString objects, each of which contains a key path to one of the document’s attributes.

## Discussion

You can use this method instead of, or in addition to, the encodeRestorableState(with:) and restoreState(with:) methods to save and restore the state of your document. The key paths must refer to attributes that are Key-value coding and Key-value observing compliant.

When changes are detected, the specified attributes are automatically written to disk with the rest of the app’s interface-related state. At launch time, the attributes are automatically restored to their previous values.

## See Also

### Handling Window Restoration

class func allowedClasses(forRestorableStateKeyPath: String) -> [AnyClass]

Returns the classes that support secure coding.

func encodeRestorableState(with: NSCoder)

Saves the interface-related state of the document.

func restoreState(with: NSCoder)

Restores the interface-related state of the document.

func invalidateRestorableState()

Marks the document’s interface-related state as dirty.

func restoreWindow(withIdentifier: NSUserInterfaceItemIdentifier, state: NSCoder, completionHandler: (NSWindow?, (any Error)?) -> Void)

Restores a window that was associated with a document, after that document is reopened.

