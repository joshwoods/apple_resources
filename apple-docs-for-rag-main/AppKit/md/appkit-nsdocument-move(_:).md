

- AppKit
- NSDocument
-  move(\_:) 

Instance Method

# move(\_:)

Moves the document to a new location in response to the user choosing the Move To… menu item.

macOS 10.8+

``` source
@IBAction @MainActor
func move(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

This is the action method of the Move To… menu item in a document-based app. By default, this method invokes the move(completionHandler:) method, passing `nil` as a parameter value.

## See Also

### Moving the Document

func move(completionHandler: ((Bool) -> Void)?)

Moves the document to a user-selected location.

func move(to: URL, completionHandler: (((any Error)?) -> Void)?)

Moves the document’s file to the given URL.

