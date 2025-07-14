

- AppKit
- NSDocument
-  lock(completionHandler:) 

Instance Method

# lock(completionHandler:)

Prevents the user from making further changes to the document.

macOS 10.8+

``` source
@MainActor
func lock(completionHandler: ((Bool) -> Void)? = nil)
```

``` source
@MainActor
func lock() async -> Bool
```

## Parameters 

`completionHandler`  

The completion handler block object passed in to be invoked after locking is completed, regardless of success or failure of locking.

## Discussion

By default, this method first ensures that any editor who has registered using Cocoa Binding’s NSEditorRegistration informal protocol has committed all changes and then autosaves the document, if necessary, before attempting to lock it using the lock(completionHandler:) method. Upon successful locking, the isLocked property is set to `[YES]`. Documents whose fileURL property is set to `nil` cannot be locked.

## See Also

### Locking the Document

func lock(Any?)

Locks the document in response to the user choosing the Lock menu item.

func unlock(Any?)

Unlocks the document in response to the user choosing the Unlock menu item.

func lock(completionHandler: (((any Error)?) -> Void)?)

Prevents the user from making changes to the document’s file.

func unlock(completionHandler: ((Bool) -> Void)?)

Allows the user to make modifications to the document.

func unlock(completionHandler: (((any Error)?) -> Void)?)

Allows the user to make modifications to the document’s file.

var isLocked: Bool

A Boolean value that indicates whether or not the file can be written to.

