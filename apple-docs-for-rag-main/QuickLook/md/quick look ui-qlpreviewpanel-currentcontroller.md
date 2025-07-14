

- Quick Look UI
- QLPreviewPanel
-  currentController 

Instance Property

# currentController

The current first responder accepting to control the preview panel.

macOS 10.6+

``` source
@MainActor
var currentController: Any! { get }
```

## Discussion

You should never change the preview panel’s state (for example, its delegate, datasource, and so on) if you aren’t controlling it.

## See Also

### Accessing the Preview Panel Controller

func updateController()

Asks the preview panel to update its current controller.

