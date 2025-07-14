

- Quick Look UI
- QLPreviewPanelDataSource
-  previewPanel(\_:previewItemAt:) 

Instance Method

# previewPanel(\_:previewItemAt:)

Returns the item that the preview panel should preview at a given index.

macOS 10.6+

``` source
func previewPanel(
    _ panel: QLPreviewPanel!,
    previewItemAt index: Int
) -> (any QLPreviewItem)!
```

**Required**

## Parameters 

`panel`  

The preview panel.

`index`  

The index of the item to preview.

## Return Value

The item that the preview panel should preview at index `index`.

## See Also

### Required Methods

func numberOfPreviewItems(in: QLPreviewPanel!) -> Int

Returns the number of items that the preview panel should preview.

**Required**

