

- AppKit
- NSDocument
-  isLocked 

Instance Property

# isLocked

A Boolean value that indicates whether or not the file can be written to.

macOS 10.8+

``` source
@MainActor
var isLocked: Bool { get }
```

## Discussion

This property may contain the value true because the user lacks the appropriate write permissions, the “user immutable” flag was raised, the parent directory or volume is read only, or the checkAutosavingSafety() method returned false. Do not override this property.

## See Also

### Locking the Document

func lock(Any?)

Locks the document in response to the user choosing the Lock menu item.

func unlock(Any?)

Unlocks the document in response to the user choosing the Unlock menu item.

func lock(completionHandler: ((Bool) -> Void)?)

Prevents the user from making further changes to the document.

func lock(completionHandler: (((any Error)?) -> Void)?)

Prevents the user from making changes to the document’s file.

func unlock(completionHandler: ((Bool) -> Void)?)

Allows the user to make modifications to the document.

func unlock(completionHandler: (((any Error)?) -> Void)?)

Allows the user to make modifications to the document’s file.

