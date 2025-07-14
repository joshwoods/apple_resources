

- AppKit
- NSDocument
-  encodeRestorableState(with:backgroundQueue:) 

Instance Method

# encodeRestorableState(with:backgroundQueue:)

Saves the interface-related state of the document.

macOS 10.13+

``` source
@MainActor
func encodeRestorableState(
    with coder: NSCoder,
    backgroundQueue queue: OperationQueue
)
```

## Parameters 

`coder`  

The coder object in which to save the responder’s interface-related state.

`queue`  

A serial background operation queue on which to encode additional state asynchronously.

## Discussion

This method is part of the window restoration system and is called at appropriate times to save the visual state of your responder to the specified archive. The default implementation of this method does nothing but specific subclasses (such as NSView and NSWindow) override it to save important state information. Therefore, if you override this method, always call `super` at some point in your implementation.

Subclasses can override this method and use it to restore any information that would be needed to restore the responder to its current state. For example, the NSTabView class uses this method to save information about the currently selected tab. You must store enough data to reconfigure the responder and return it to its current state during a subsequent launch of the application.

AppKit calls this method on your app’s main thread. If you want to encode any state information asynchronously on a background thread, submit one or more operation objects to the provided `queue`. Performing long-running operations asynchronously lets you free up the main thread for other operations more quickly. The encoding operation is not considered final until all operations submitted to `queue` finish.

For information about using a coder object to write data to an archive, see Archives and Serializations Programming Guide.

## See Also

### Managing Document Windows

func showWindows()

Displays all of the document’s windows, bringing them to the front and making them main or key as necessary.

func setWindow(NSWindow?)

Sets the window outlet of this document to the specified value.

var windowForSheet: NSWindow?

Returns the document window to use as the parent of a document-modal sheet.

var displayName: String!

The name of the document as displayed in the title bars of the document’s windows and in alert dialogs related to the document.

func defaultDraftName() -> String

Returns the default draft name for the document subclass.

