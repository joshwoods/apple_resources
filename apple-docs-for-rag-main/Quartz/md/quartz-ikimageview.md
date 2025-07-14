

- Quartz
-  IKImageView 

Class

# IKImageView

A view that allows displaying and minor editing of an image.

macOS 10.5+

``` source
@MainActor
class IKImageView
```

## Overview

The `IKImageView` class provides an efficient way to display images in a view while at the same time supporting a number of image editing operations such as rotating, zooming, and cropping. If possible, image rendering uses hardware acceleration to achieve optimal performance. The `IKImageView` class is implemented as a subclass of NSView. Similar to NSImageView, the `IKImageView` class is used to display a single image.

You can provide an images for the view in any of these formats:

- File reference (NSURL, CFURL, or a path)

- CGImageSource

- Data (NSData or CFData)

- Image (CGImage or CIImage)

Providing a file reference is the preferred way to set the the image for a view because in addition to the actual image data, `IKImageView` also handles the image metadata embedded in the file. The image view automatically fetches the metadata from a file reference, whereas for the other sources (except for a CGImageSource source), it cannot. For images set from other sources, you need to set the metadata separately.

`IKImageView` supports multi-frame images (TIFF, GIF, and so forth) and animated images.

## Topics

### Getting and Setting Image View Characteristics

var delegate: AnyObject!

Specifies the delegate object of the receiver.

var zoomFactor: CGFloat

Specifies the zoom factor for the image view.

var rotationAngle: CGFloat

Specifies the rotation angle for the image view.

var currentToolMode: String!

Specifies the current tool mode for the image view.

var autoresizes: Bool

Specifies the automatic resizing state for the image view.

var hasHorizontalScroller: Bool

Specifies the horizontal scroll bar state for the image view.

var hasVerticalScroller: Bool

Specifies the vertical scroll bar state for the image view.

var autohidesScrollers: Bool

Specifies the automatic-hiding scroll bar state for the image view.

var supportsDragAndDrop: Bool

Specifies the drag-and-drop support state for the image view.

var editable: Bool

Specifies the editable state for the image view.

var doubleClickOpensImageEditPanel: Bool

Specifies the image-opening state of the editing pane in the image view.

var imageCorrection: CIFilter!

Specifies a Core Image filter for image correction.

var backgroundColor: NSColor!

Specifies the background color for the image view.

func imageSize() -> NSSize

Returns the size of the image in the image view.

func imageProperties() -> [AnyHashable : Any]!

Returns the metadata for the image in the view.

### Getting and Setting Images

func image() -> Unmanaged&lt;CGImage>!

Returns the image associated with the view, after any image corrections.

func setImage(CGImage!, imageProperties: [AnyHashable : Any]!)

Sets the image to display in an image view.

func setImageWith(URL!)

Initializes an image view with the image specified by a URL.

### Manipulating the Image in a View

func setRotationAngle(CGFloat, center: NSPoint)

Sets the rotation angle at the provided origin.

func setImageZoomFactor(CGFloat, center: NSPoint)

Sets the zoom factor at the provided origin.

func zoomImageToFit(Any!)

Zooms the image so that it fits in the image view.

func zoomImageToActualSize(Any!)

Zooms the image so that it is displayed using its true size.

func zoomImage(to: NSRect)

Zooms the image so that it fits in the specified rectangle.

func zoomIn(Any!)

Zooms the image in.

func zoomOut(Any!)

Zooms the image out.

func crop(Any!)

Crops the image using the current selection.

func flipImageHorizontal(Any!)

Flips an image along the horizontal axis.

func flipImageVertical(Any!)

Flips an image along the vertical axis.

func rotateImageLeft(Any!)

Rotates the image left (counter-clockwise).

func rotateImageRight(Any!)

Rotates the image right (clockwise).

### Working With Core Animation

func setOverlay(CALayer!, forType: String!)

Sets an overlay type for a Core Animation layer.

func overlay(forType: String!) -> CALayer!

Returns the Core Animation layer associated with a layer type.

### Scrolling

func scroll(to: NSPoint)

Scrolls the view to the specified point.

func scroll(to: NSRect)

Scrolls the view so that it includes the provided rectangular area.

### Converting Points and Rectangles

func convertPoint(toImagePoint: NSPoint) -> NSPoint

Converts an image view coordinate to an image coordinate.

func convertRect(toImageRect: NSRect) -> NSRect

Converts an image view rectangle to an image rectangle.

func convertImagePoint(toViewPoint: NSPoint) -> NSPoint

Converts an image coordinate to an image view coordinate.

func convertImageRect(toViewRect: NSRect) -> NSRect

Converts an image rectangle to an image view rectangle.

### Constants

Tool Modes

Image Kit tools modes referenced by the currentToolMode property.

Overlay Types

A layer level.

## Relationships

### Inherits From

- NSView

### Conforms To

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
- Sendable

## See Also

### Classes

class IKCameraDeviceView

The `IKCameraDeviceView` class displays the contents of the selected camera.

class IKDeviceBrowserView

The `IKDeviceBrowserView` allows you to select a camera or scanner from a list of the available devices.

class IKFilterBrowserPanel

Presents a user interface for browsing filters.

class IKFilterBrowserView

The `IKFilterBrowserView` class is used as a container for the elements of an IKFilterBrowserPanel object.

class IKFilterUIView

Input parameters for filtering core image filters.

class IKImageBrowserCell

A class used to display a cell.

class IKImageEditPanel

The `IKImageEditPanel` class provides a panel, that is, a utility window that floats on top of document windows, optimized for image editing.

class IKPictureTaker

The `IKPictureTaker` class represents a panel that allows users to choose images by browsing the file system. The picture taker panel provides an Open Recent menu, supports image cropping, and supports taking snapshots from an iSight or other digital camera.

class IKSaveOptions

The `IKSaveOptions` class initializes, adds, and manages user interface options for saving image data.

class IKScannerDeviceView

The `IKScannerDeviceView` class displays a view that allows scanning. It can be customized by specifying the display mode. The delegate receives the scanned data and must implement the IKScannerDeviceViewDelegate protocol.

class IKSlideshow

The `IKSlideshow` class encapsulates a data source and options for a slideshow.

