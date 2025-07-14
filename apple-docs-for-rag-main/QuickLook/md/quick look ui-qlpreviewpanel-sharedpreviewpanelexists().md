

- Quick Look UI
- QLPreviewPanel
-  sharedPreviewPanelExists() 

Type Method

# sharedPreviewPanelExists()

Returns a Boolean value that indicates whether the system has created a shared Quick Look preview panel.

macOS 10.6+

``` source
@MainActor
class func sharedPreviewPanelExists() -> Bool
```

## Return Value

true if the shared Quick Look preview panel instance has been created, otherwise false.

## See Also

### Accessing the Shared Panel

class func shared() -> QLPreviewPanel!

Returns the shared Quick Look preview panel instance.

