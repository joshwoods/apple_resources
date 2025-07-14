

- AppKit
- NSDocument
-  unlock(completionHandler:) 

Instance Method

# unlock(completionHandler:)

Allows the user to make modifications to the document.

macOS 10.8+

``` source
@MainActor
func unlock(completionHandler: ((Bool) -> Void)? = nil)
```

``` source
@MainActor
func unlock() async -> Bool
```

## Parameters 

`completionHandler`  

The completion handler block object passed in to be invoked after unlocking is completed, regardless of success or failure.

## Discussion

By default, this method invokes the unlock(completionHandler:) method to unlock the document. This method disables autosaving safety checking, meaning that checkAutosavingSafety() will no longer be invoked on this document. When unlocking succeeds, the isLocked method will begin returning false.

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

func unlock(completionHandler: (((any Error)?) -> Void)?)

Allows the user to make modifications to the document’s file.

var isLocked: Bool

A Boolean value that indicates whether or not the file can be written to.

