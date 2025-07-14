

- WebKit
- WebUIDelegate
-  webView(\_:willPerform:from:with:) Deprecated

Instance Method

# webView(\_:willPerform:from:with:)

Tells the receiver that the sending web view will perform the specified drag-source action.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    willPerform action: WebDragSourceAction,
    from point: NSPoint,
    with pasteboard: NSPasteboard!
)
```

## Parameters 

`webView`  

The web view that sent the message.

`action`  

The drag-source action to perform. See WebDragSourceAction for a list of actions.

`point`  

The point at which the drag began, specified in the coordinates of the web view.

`pasteboard`  

The drag pasteboard.

## Discussion

This method is invoked after the last invocation of the webView(_:dragSourceActionMaskFor:) method, when the dragged content is dropped and the sender is about to perform the drag-source action. The delegate has the opportunity to modify the contents of the object on the pasteboard before completing the drag-source action. No action is taken if you do not implement this method.

## See Also

### Controlling Drag Behavior

func webView(WebView!, dragDestinationActionMaskFor: (any NSDraggingInfo)!) -> Int

Returns a mask indicating which drag operations are allowed by the sender.

Deprecated

func webView(WebView!, dragSourceActionMaskFor: NSPoint) -> Int

Returns a mask indicating which drag-source actions are allowed for a drag that begins at the specified location.

Deprecated

func webView(WebView!, willPerform: WebDragDestinationAction, for: (any NSDraggingInfo)!)

Tells the receiver that the sending web view will perform the specified drag-destination action.

Deprecated

