

- AppKit
- NSDocument
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

Saves the interface-related state of the document.

func restoreState(with: NSCoder)

Restores the interface-related state of the document.

class var restorableStateKeyPaths: [String]

Returns an array of key paths that represent the restorable attributes of the document.

func invalidateRestorableState()

Marks the document’s interface-related state as dirty.

func restoreWindow(withIdentifier: NSUserInterfaceItemIdentifier, state: NSCoder, completionHandler: (NSWindow?, (any Error)?) -> Void)

Restores a window that was associated with a document, after that document is reopened.

