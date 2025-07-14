

- Quartz
- IKImageView
-  imageCorrection 

Instance Property

# imageCorrection

Specifies a Core Image filter for image correction.

macOS 10.5+

``` source
@MainActor
unowned(unsafe) var imageCorrection: CIFilter! { get set }
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

var supportsDragAndDrop: Bool

Specifies the drag-and-drop support state for the image view.

var editable: Bool

Specifies the editable state for the image view.

var doubleClickOpensImageEditPanel: Bool

Specifies the image-opening state of the editing pane in the image view.

var backgroundColor: NSColor!

Specifies the background color for the image view.

func imageSize() -> NSSize

Returns the size of the image in the image view.

func imageProperties() -> [AnyHashable : Any]!

Returns the metadata for the image in the view.

