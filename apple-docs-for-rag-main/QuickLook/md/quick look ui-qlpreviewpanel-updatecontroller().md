

- Quick Look UI
- QLPreviewPanel
-  updateController() 

Instance Method

# updateController()

Asks the preview panel to update its current controller.

macOS 10.6+

``` source
@MainActor
func updateController()
```

## Discussion

The preview panel automatically updates its controller (by searching the responder chain) whenever the main or key window changes. You should only invoke this method if the responder chain changes without explicit notice.

## See Also

### Accessing the Preview Panel Controller

var currentController: Any!

The current first responder accepting to control the preview panel.

