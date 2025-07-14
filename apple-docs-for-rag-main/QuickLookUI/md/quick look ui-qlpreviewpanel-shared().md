

- Quick Look UI
- QLPreviewPanel
-  shared() 

Type Method

# shared()

Returns the shared Quick Look preview panel instance.

macOS 10.6+

``` source
@MainActor
class func shared() -> QLPreviewPanel!
```

## Return Value

The shared Quick Look preview panel instance for the application.

## Discussion

This method creates the panel if it doesn’t exist yet. Use sharedPreviewPanelExists() if you want to determine whether the panel exists without creating it.

## See Also

### Accessing the Shared Panel

class func sharedPreviewPanelExists() -> Bool

Returns a Boolean value that indicates whether the system has created a shared Quick Look preview panel.

