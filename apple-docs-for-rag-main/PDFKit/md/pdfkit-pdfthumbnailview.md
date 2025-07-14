

- PDFKit
-  PDFThumbnailView 

Class

# PDFThumbnailView

An object that contains a set of thumbnails, each of which represents a page in a PDF document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class PDFThumbnailView
```

## Topics

### Accessing the Associated PDF View

var pdfView: PDFView?

Returns the `PDFView` object associated with the thumbnail view.

### Managing the Size of a Thumbnail View

var thumbnailSize: CGSize

Returns the maximum width and height of the thumbnails in the thumbnail view.

### Working with Thumbnail View Display Characteristics

var maximumNumberOfColumns: Int

Returns the maximum number of columns of thumbnails the thumbnail view can display.

var labelFont: NSFont?

Returns the font used to label the thumbnails.

var backgroundColor: UIColor?

Returns the color used in the background of the thumbnail view.

### Managing the Behavior of a Thumbnail View

var allowsDragging: Bool

Returns a Boolean value indicating whether users can drag thumbnails (that is, re-order pages in the document) within the thumbnail view.

var allowsMultipleSelection: Bool

Returns a Boolean value indicating whether users can select multiple thumbnails in the thumbnail view at one time.

var selectedPages: [PDFPage]?

Returns an array of PDF pages that correspond to the selected thumbnails in the thumbnail view.

### Instance Properties

var contentInset: UIEdgeInsets

var layoutMode: PDFThumbnailLayoutMode

## Relationships

### Inherits From

- NSView
- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Views

class PDFView

An object that encapsulates the functionality of PDF Kit into a single widget that you can add to your application using Interface Builder.

