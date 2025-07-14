

- Quartz
- IKImageView
-  supportsDragAndDrop 

Instance Property

# supportsDragAndDrop

Specifies the drag-and-drop support state for the image view.

macOS 10.5+

``` source
@MainActor
var supportsDragAndDrop: Bool { get set }
```

## See Also

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

