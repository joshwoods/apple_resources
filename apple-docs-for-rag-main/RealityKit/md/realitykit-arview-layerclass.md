

- RealityKit
- ARView
-  layerClass 

Type Property

# layerClass

The class used to create the layer for view instances.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+

``` source
@MainActor @preconcurrency
override dynamic class var layerClass: AnyClass { get }
```

## See Also

### Managing the view

var frame: NSRect

The frame rectangle, which describes the view’s location and size in the coordinate system of the view’s superview.

var contentScaleFactor: CGFloat

The scale factor of the content in the view.

func didMoveToSuperview()

Tells the view that its superview changed.

func didMoveToWindow()

Tells the view that its window property is set to a new value.

func layoutSubviews()

Lays out subviews.

func layout()

func makeBackingLayer() -> CALayer

Creates the view’s backing layer.

func viewDidChangeBackingProperties()

Tells the view when its backing store properties change.

func viewDidMoveToSuperview()

Tells the view that it has a new superview or that the view’s superview has been removed.

