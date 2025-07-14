

- AppKit
- NSDocument
-  unlock(\_:) 

Instance Method

# unlock(\_:)

Unlocks the document in response to the user choosing the Unlock menu item.

macOS 10.8+

``` source
@IBAction @MainActor
func unlock(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

This is the action of the Unlock menu item in a document-based app. This action method invokes the unlock(completionHandler:) method by default.

## See Also

### Locking the Document

func lock(Any?)

Locks the document in response to the user choosing the Lock menu item.

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

