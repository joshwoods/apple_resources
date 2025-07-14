

- Quick Look UI
-  QLPreviewItemLoadingBlock Deprecated

Type Alias

# QLPreviewItemLoadingBlock

A type that defines a block used to load a Quick Look preview item.

macOS 10.13–10.14Deprecated

``` source
typealias QLPreviewItemLoadingBlock = ((any Error)?) -> Void
```

Deprecated

Use void (^)(NSError \* \_Nullable) instead

## Discussion

A type that defines a block used to load a Quick Look preview item.

## See Also

### Previews

class QLPreviewPanel

A class that implements the Quick Look preview panel to display a preview of a list of items.

class QLPreviewView

A Quick Look preview of an item that you can embed into your view hierarchy.

protocol QLPreviewItem

A protocol that defines a set of properties you implement to make a preview of your application’s content.

protocol QLPreviewPanelDataSource

A protocol that the Quick Look preview panel uses to access the contents of its data source object.

protocol QLPreviewPanelDelegate

A protocol for the delegate of the Quick Look preview panel.

