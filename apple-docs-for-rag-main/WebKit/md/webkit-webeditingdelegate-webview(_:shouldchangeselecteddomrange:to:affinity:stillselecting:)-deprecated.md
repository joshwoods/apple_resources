

- WebKit
- WebEditingDelegate
-  webView(\_:shouldChangeSelectedDOMRange:to:affinity:stillSelecting:) Deprecated

Instance Method

# webView(\_:shouldChangeSelectedDOMRange:to:affinity:stillSelecting:)

Returns whether the user should be allowed to change the selected range.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    shouldChangeSelectedDOMRange currentRange: DOMRange!,
    to proposedRange: DOMRange!,
    affinity selectionAffinity: NSSelectionAffinity,
    stillSelecting flag: Bool
) -> Bool
```

## Parameters 

`webView`  

The web view that the user is editing.

`currentRange`  

The old range the user wants to change.

`proposedRange`  

The new range the user wants to select.

`selectionAffinity`  

The direction of the selection.

`flag`  

true if the user is still selecting; otherwise, false.

## Return Value

true if the user is allowed to change the selected range; otherwise, false.

## See Also

### Related Documentation

func webViewDidChangeSelection(Notification!)

Sent by the default notification center when the user changes the selection in the web view.

Deprecated

