

- Quartz
- ImageKit
-  ImageKit Constants 

API Collection

# ImageKit Constants

## Topics

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

let IKImageBrowserCellsTitleAttributesKey: String

A key for title attribute of an item in the image browser view.

let IKImageBrowserGroupBackgroundColorKey: String

A key for the background color of a group.

let IKImageBrowserGroupFooterLayer: String

A key for the header layer of the group.

let IKImageBrowserGroupHeaderLayer: String

A key for the header layer of the group.

let IKImageBrowserGroupRangeKey: String

A key for the range of a group.

let IKImageBrowserGroupStyleKey: String

A key for the style of a group.

let IKImageBrowserGroupTitleKey: String

A key for the title of a group.

let IKImageBrowserSelectionColorKey: String

A key for the color that indicates a selection.

var IKImageStateInvalid: IKImageBrowserCellState

The thumbnail is invalid. For example, an unsupported image is provided.

var IKImageStateNoImage: IKImageBrowserCellState

Returned until a thumbnail has been created from the represented object.

var IKImageStateReady: IKImageBrowserCellState

The receiver’s represented object has been set and the cell is ready to display.

let IKOverlayTypeBackground: String

A background.

let IKOverlayTypeImage: String

An image.

let IKPictureTakerAllowsEditingKey: String

A key for allowing image editing.

let IKPictureTakerAllowsFileChoosingKey: String

A key for allowing the user to choose a file.

let IKPictureTakerAllowsVideoCaptureKey: String

A key for allowing video capture.

let IKPictureTakerImageTransformsKey: String

A n image transformation key. The associated value is an `NSDictionary` object that can be serialized.

let IKPictureTakerInformationalTextKey: String

A key for informational text. The associated value is an `NSString` or `NSAttributedString` object whose default value is `"Drag Image Here"`.

let IKPictureTakerOutputImageMaxSizeKey: String

A key for the maximum size of the output image. The associated value is an `NSValue` object (`NSSize`).

let IKPictureTakerRemainOpenAfterValidateKey: String

A key that determines if the picture taker UI should remain open after the user selects done.

let IKPictureTakerShowAddressBookPicture: StringDeprecated

let IKPictureTakerShowAddressBookPictureKey: String

A key for showing the address book picture.

let IKPictureTakerShowEffectsKey: String

A key for showing effects.

let IKPictureTakerShowEmptyPicture: StringDeprecated

let IKPictureTakerShowEmptyPictureKey: String

A key for showing an empty picture. The associated value is an `NSImage` object. The default value is `nil`. If set to an image, the picture taker automatically shows an image at the end of the Recent Pictures pop-up menu. that means “no picture.”

let IKPictureTakerShowRecentPictureKey: String

let IKPictureTakerUpdateRecentPictureKey: String

A key for allowing a recent picture to be updated.

let IKSlideshowAudioFile: String

A key specifying the audio file played during the slideshow.

let IKSlideshowModeImages: String

All items in the slideshow are images.

let IKSlideshowModeOther: String

There are a mixture of items in the slideshow (image, PDF, text, HTML, and so on).

let IKSlideshowModePDF: String

All items in the slideshow are PDF documents.

let IKSlideshowPDFDisplayBox: String

A key for the PDF display box.

let IKSlideshowPDFDisplayMode: String

A key for the PDF display mode.

let IKSlideshowPDFDisplaysAsBook: String

A key for displaying the slideshow as a book. The associated value is a `Boolean` data type.

let IKSlideshowScreen: String

A key specifying the screen on which the slideshow is displayed.

let IKSlideshowStartIndex: String

A key for the slideshow item index. The associated value is an index.

let IKSlideshowStartPaused: String

A key for starting in a paused state. The associated value is a `Boolean` data type.

let IKSlideshowWrapAround: String

A key for starting the slideshow over after the last slide shows. The associated value is a `Boolean` data type.

let IKToolModeAnnotate: String

The annotation tool.

let IKToolModeCrop: String

The crop tool.

let IKToolModeMove: String

The move tool.

let IKToolModeNone: String

No tool is set.

let IKToolModeRotate: String

The rotation tool.

let IKToolModeSelect: String

The selection tool.

let IKToolModeSelectEllipse: String

The selection ellipse.

let IKToolModeSelectLasso: String

The selection lasso.

let IKToolModeSelectRect: String

Same as `IKToolModeSelect`.

let IKUIFlavorAllowFallback: String

Substitute controls of another size. The associated value is a Boolean value. If the filter cannot provide a view for the requested size and a fallback is allowed, the filter can use controls of a different size.

let IKUISizeFlavor: String

A key for the size of the controls in a filter view. The associated value can be IKUISizeMini, IKUISizeSmall, or IKUISizeRegular.

let IKUISizeMini: String

A very small control.

let IKUISizeRegular: String

A standard size control.

let IKUISizeSmall: String

A small control.

let IKUImaxSize: String

The maximum size of a filter view.

let IK_ApertureBundleIdentifier: String

The Aperature application—`com.apple.Aperture`.

let IK_MailBundleIdentifier: String

The Mail application—`com.apple.mail`.

let IK_PhotosBundleIdentifier: String

let IK_iPhotoBundleIdentifier: String

The iPhoto application—`com.apple.iPhoto`.

### Deprecated constants

let IKPictureTakerCropAreaSizeKey: String

A key for the cropping area size. The associated value is an `NSValue` object (`NSSize`).

Deprecated

let IKPictureTakerShowAddressBookPicture: StringDeprecated

let IKPictureTakerShowEmptyPicture: StringDeprecated

## See Also

### Reference

Quartz Enumerations

