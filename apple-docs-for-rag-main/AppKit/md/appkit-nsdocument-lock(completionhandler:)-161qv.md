

- AppKit
- NSDocument
-  lock(completionHandler:) 

Instance Method

# lock(completionHandler:)

Prevents the user from making changes to the document’s file.

macOS 10.8+

``` source
@MainActor
func lock(completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
@MainActor
func lock() async throws
```

## Parameters 

`completionHandler`  

The completion handler block object passed in to be invoked after locking is completed, regardless of success or failure of locking.

## Discussion

This method first locks the file at `[self fileURL]` and then invokes the given block. The default locking implementation is to enable the “user immutable” flag on the file.

## See Also

### Locking the Document

func lock(Any?)

Locks the document in response to the user choosing the Lock menu item.

func unlock(Any?)

Unlocks the document in response to the user choosing the Unlock menu item.

func lock(completionHandler: ((Bool) -> Void)?)

Prevents the user from making further changes to the document.

func unlock(completionHandler: ((Bool) -> Void)?)

Allows the user to make modifications to the document.

func unlock(completionHandler: (((any Error)?) -> Void)?)

Allows the user to make modifications to the document’s file.

var isLocked: Bool

A Boolean value that indicates whether or not the file can be written to.

