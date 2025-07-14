

- WebKit
- WebUIDelegate
-  webView(\_:willPerform:for:) Deprecated

Instance Method

# webView(\_:willPerform:for:)

Tells the receiver that the sending web view will perform the specified drag-destination action.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    willPerform action: WebDragDestinationAction,
    for draggingInfo: (any NSDraggingInfo)!
)
```

## Parameters 

`webView`  

The web view that sent the message.

`action`  

The drag-destination action to perform. See WebDragDestinationAction for a list of actions.

`draggingInfo`  

The information object for the dragging operation.

## Discussion

This method is invoked after the last invocation of the webView(_:dragDestinationActionMaskFor:) method, when the dragged content is dropped and the sender is about to perform the destination action. No action is taken if you do not implement this method.

## See Also

### Controlling Drag Behavior

func webView(WebView!, dragDestinationActionMaskFor: (any NSDraggingInfo)!) -> Int

Returns a mask indicating which drag operations are allowed by the sender.

Deprecated

func webView(WebView!, dragSourceActionMaskFor: NSPoint) -> Int

Returns a mask indicating which drag-source actions are allowed for a drag that begins at the specified location.

Deprecated

func webView(WebView!, willPerform: WebDragSourceAction, from: NSPoint, with: NSPasteboard!)

Tells the receiver that the sending web view will perform the specified drag-source action.

Deprecated

