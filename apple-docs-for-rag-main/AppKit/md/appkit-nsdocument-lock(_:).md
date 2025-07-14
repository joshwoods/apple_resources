

- AppKit
- NSDocument
-  lock(\_:) 

Instance Method

# lock(\_:)

Locks the document in response to the user choosing the Lock menu item.

macOS 10.8+

``` source
@IBAction @MainActor
func lock(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

This is the action of the Lock menu item in a document-based app. This action method invokes the lock(completionHandler:) method by default.

## See Also

### Locking the Document

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

var isLocked: Bool

A Boolean value that indicates whether or not the file can be written to.

