

- AppKit
- NSDocument
-  move(completionHandler:) 

Instance Method

# move(completionHandler:)

Moves the document to a user-selected location.

macOS 10.8+

``` source
@MainActor
func move(completionHandler: ((Bool) -> Void)? = nil)
```

``` source
@MainActor
func move() async -> Bool
```

## Parameters 

`completionHandler`  

The completion handler block object passed in to be invoked after moving is completed, regardless of success, failure, or cancellation of moving action.

## Discussion

This method presents the user with a move panel if `[self fileURL]` is non-nil and then tries to save the document to the new location by invoking the move(to:completionHandler:) method if the user accepts the location presented by the panel. If a file with the same name already exists at that location, the user will be asked to choose between replacing the pre-existing file, renaming the current document, or canceling the move process. If `[self fileURL]` is `nil`, then the `[self runModalSavePanelForSaveOperation:NSSaveAsOperation delegate:didSaveSelector:contextInfo:]` message is sent instead.

## See Also

### Related Documentation

func moveToUbiquityContainer(Any?)

Moves the document to the user’s iCloud storage.

### Moving the Document

func move(Any?)

Moves the document to a new location in response to the user choosing the Move To… menu item.

func move(to: URL, completionHandler: (((any Error)?) -> Void)?)

Moves the document’s file to the given URL.

