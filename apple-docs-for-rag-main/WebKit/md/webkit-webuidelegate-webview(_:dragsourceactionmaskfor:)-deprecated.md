

- WebKit
- WebUIDelegate
-  webView(\_:dragSourceActionMaskFor:) Deprecated

Instance Method

# webView(\_:dragSourceActionMaskFor:)

Returns a mask indicating which drag-source actions are allowed for a drag that begins at the specified location.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    dragSourceActionMaskFor point: NSPoint
) -> Int
```

## Parameters 

`webView`  

The web view that sent the message.

`point`  

The point at which the drag began, specified in the coordinates of the web view.

## Return Value

A mask indicating which drag-source actions are allowed. (Note that the return value changed from an `unsigned int` to an `NSUInteger` in OS X v10.5.) See WebDragSourceAction for a list of return values.

## Discussion

This method is called after the user has begun a drag from a point in a web view. This method can be invoked multiple times while content is dragged from the sending web view. When the content is dropped, the sender sends webView(_:willPerform:from:with:) to the receiver.

If you do not implement this method, it returns `(WebDragSourceActionAny & ~WebDragSourceActionLink)` if the cursor is in an editable part of the web view; otherwise, it returns any.

## See Also

### Controlling Drag Behavior

func webView(WebView!, dragDestinationActionMaskFor: (any NSDraggingInfo)!) -> Int

Returns a mask indicating which drag operations are allowed by the sender.

Deprecated

func webView(WebView!, willPerform: WebDragDestinationAction, for: (any NSDraggingInfo)!)

Tells the receiver that the sending web view will perform the specified drag-destination action.

Deprecated

func webView(WebView!, willPerform: WebDragSourceAction, from: NSPoint, with: NSPasteboard!)

Tells the receiver that the sending web view will perform the specified drag-source action.

Deprecated

