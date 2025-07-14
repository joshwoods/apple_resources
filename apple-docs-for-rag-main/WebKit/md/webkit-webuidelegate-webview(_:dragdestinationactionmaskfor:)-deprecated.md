

- WebKit
- WebUIDelegate
-  webView(\_:dragDestinationActionMaskFor:) Deprecated

Instance Method

# webView(\_:dragDestinationActionMaskFor:)

Returns a mask indicating which drag operations are allowed by the sender.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    dragDestinationActionMaskFor draggingInfo: (any NSDraggingInfo)!
) -> Int
```

## Parameters 

`webView`  

The web view that sent the message.

`draggingInfo`  

The information object for the dragging operation.

## Return Value

A mask that indicates which drag operations are allowed when content is dragged over the sending web view. (Note that the return value changed from an `unsigned int` to an `NSUInteger` in OS X v10.5.) See WebDragDestinationAction for a list of return values.

## Discussion

This method can be invoked multiple times while content is dragged over the sending web view. When the content is dropped, the web view sends a notification (webView(_:willPerform:for:)) to the receiver.

If you do not implement this method, it returns any by default.

## See Also

### Controlling Drag Behavior

func webView(WebView!, dragSourceActionMaskFor: NSPoint) -> Int

Returns a mask indicating which drag-source actions are allowed for a drag that begins at the specified location.

Deprecated

func webView(WebView!, willPerform: WebDragDestinationAction, for: (any NSDraggingInfo)!)

Tells the receiver that the sending web view will perform the specified drag-destination action.

Deprecated

func webView(WebView!, willPerform: WebDragSourceAction, from: NSPoint, with: NSPasteboard!)

Tells the receiver that the sending web view will perform the specified drag-source action.

Deprecated

