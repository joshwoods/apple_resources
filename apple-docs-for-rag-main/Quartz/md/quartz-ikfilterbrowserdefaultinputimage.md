

- Quartz
-  IKFilterBrowserDefaultInputImage 

Global Variable

# IKFilterBrowserDefaultInputImage

The key for the default input image.

macOS 10.4+

``` source
let IKFilterBrowserDefaultInputImage: String
```

## Discussion

The associated value is the CIImage object to use as the default input image for the filter preview. Setting the image to `nil` causes Image Kit to use the image supplied by the framework. You can also set the input image and other parameters during the notification IKFilterBrowserWillPreviewFilterNotification.

## See Also

### Constants

var IKImageBrowserDropOn: IKImageBrowserDropOperation

Drop the item on the cell.

var IKImageBrowserDropBefore: IKImageBrowserDropOperation

Drop the item before the cell.

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

let IKImageBrowserCellsTitleAttributesKey: String

A key for title attribute of an item in the image browser view.

