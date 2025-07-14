

- AppKit
- NSDocument
-  shouldCloseWindowController(\_:delegate:shouldClose:contextInfo:) 

Instance Method

# shouldCloseWindowController(\_:delegate:shouldClose:contextInfo:)

Determines whether the system should close the document and its associated window.

macOS

``` source
@MainActor
func shouldCloseWindowController(
    _ windowController: NSWindowController,
    delegate: Any?,
    shouldClose shouldCloseSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`windowController`  

The window controller that is closed.

`delegate`  

The delegate to which the selector message is sent.

`shouldCloseSelector`  

The selector of the message sent to the delegate.

`contextInfo`  

Object passed with the callback to provide any additional context information.

## Discussion

If the window controller is the document’s last one, or is marked as causing the document to close, this method calls the method in the `shouldCloseSelector` parameter with the result of canClose(withDelegate:shouldClose:contextInfo:). In all other cases, this method calls `shouldCloseSelector` with true. This method is called automatically by NSWindow for any window that has a window controller and a document associated with it. `NSWindow` calls this method prior to sending its `delegate` the windowShouldClose(_:) message. Pass the `contextInfo` object with the callback.

The `shouldCloseSelector` callback method should have the following signature:

```
- (void)document:(NSDocument *)document shouldClose:(BOOL)shouldClose  contextInfo:(void  *)contextInfo
```

## See Also

### Creating and Managing Window Controllers

func makeWindowControllers()

Creates the window controller objects that the document uses to display its content.

func addWindowController(NSWindowController)

Adds the specified window controller to the current document.

func removeWindowController(NSWindowController)

Removes the specified window controller from the receiver’s array of window controllers.

var windowControllers: [NSWindowController]

The document’s current window controllers.

var windowNibName: NSNib.Name?

The name of the document’s sole nib file.

func windowControllerDidLoadNib(NSWindowController)

Called after one of the document’s window controllers loads its nib file.

func windowControllerWillLoadNib(NSWindowController)

Called before one of the document’s window controllers loads its nib file.

