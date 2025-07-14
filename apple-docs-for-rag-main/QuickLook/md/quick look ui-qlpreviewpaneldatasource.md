

- Quick Look UI
-  QLPreviewPanelDataSource 

Protocol

# QLPreviewPanelDataSource

A protocol that the Quick Look preview panel uses to access the contents of its data source object.

macOS 12.0+

``` source
protocol QLPreviewPanelDataSource
```

## Topics

### Required Methods

func numberOfPreviewItems(in: QLPreviewPanel!) -> Int

Returns the number of items that the preview panel should preview.

**Required**

func previewPanel(QLPreviewPanel!, previewItemAt: Int) -> (any QLPreviewItem)!

Returns the item that the preview panel should preview at a given index.

**Required**

## See Also

### Previews

class QLPreviewPanel

A class that implements the Quick Look preview panel to display a preview of a list of items.

class QLPreviewView

A Quick Look preview of an item that you can embed into your view hierarchy.

protocol QLPreviewItem

A protocol that defines a set of properties you implement to make a preview of your application’s content.

protocol QLPreviewPanelDelegate

A protocol for the delegate of the Quick Look preview panel.

typealias QLPreviewItemLoadingBlock

A type that defines a block used to load a Quick Look preview item.

Deprecated

