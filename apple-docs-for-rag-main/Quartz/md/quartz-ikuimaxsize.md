

- Quartz
-  IKUImaxSize 

Global Variable

# IKUImaxSize

The maximum size of a filter view.

macOS 10.4+

``` source
let IKUImaxSize: String
```

## Discussion

Controls whose dimensions are the maximum allowable for the filter view.A width or height of `0` indicates that dimension of the view is not restricted. If the size requested is too small, the filter is expected to return a view as small as possible. It is up to the client to verify that the returned view fits into the context.

## See Also

### Constants

var IKImageBrowserDropOn: IKImageBrowserDropOperation

Drop the item on the cell.

var IKImageBrowserDropBefore: IKImageBrowserDropOperation

Drop the item before the cell.

let IKFilterBrowserDefaultInputImage: String

The key for the default input image.

let IKFilterBrowserExcludeCategories: String

The key for excluding filter categories.

let IKFilterBrowserExcludeFilters: String

The key for excluding filters.

let IKFilterBrowserShowCategories: String

The key for showing categories. The associated value is a `BOOL` value that determines if the filter browser should show the category list.

let IKFilterBrowserShowPreview: String

The associated value is a `BOOL` value that determines if the filter browser should provide a preview.

let IKImageBrowserBackgroundColorKey: String

A key for the background color of the image browser view.

let IKImageBrowserCellBackgroundLayer: String

Layer displayed in the background.

let IKImageBrowserCellForegroundLayer: String

Layer displayed in the foreground.

let IKImageBrowserCellPlaceHolderLayer: String

Layer displayed as a placeholder when an image is not yet available.

let IKImageBrowserCellSelectionLayer: String

Layer displayed as the selection.

let IKImageBrowserCellsHighlightedTitleAttributesKey: String

A key for the highlighted title attribute for an item in the image browser view.

let IKImageBrowserCellsOutlineColorKey: String

A key for the outline color for an item in the image browser view.

let IKImageBrowserCellsSubtitleAttributesKey: String

A key for a subtitle attribute for an item in the image browser view.

