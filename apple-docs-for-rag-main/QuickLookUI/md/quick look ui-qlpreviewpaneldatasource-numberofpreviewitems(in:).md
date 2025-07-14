

- Quick Look UI
- QLPreviewPanelDataSource
-  numberOfPreviewItems(in:) 

Instance Method

# numberOfPreviewItems(in:)

Returns the number of items that the preview panel should preview.

macOS 10.6+

``` source
func numberOfPreviewItems(in panel: QLPreviewPanel!) -> Int
```

**Required**

## Parameters 

`panel`  

The preview panel.

## Return Value

The number of items the preview panel should display.

## See Also

### Required Methods

func previewPanel(QLPreviewPanel!, previewItemAt: Int) -> (any QLPreviewItem)!

Returns the item that the preview panel should preview at a given index.

**Required**

