

- Quick Look UI
- QLPreviewPanel
-  delegate 

Instance Property

# delegate

The delegate object that controls the preview panel’s behavior.

macOS 10.6+

``` source
@MainActor
unowned(unsafe) var delegate: AnyObject! { get set }
```

## Discussion

The class assigned as the delegate should conform to the QLPreviewPanelDelegate protocol.

