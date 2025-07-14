

- Core Animation
- CALayer
-  delegate 

Instance Property

# delegate

The layer’s delegate object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
weak var delegate: (any CALayerDelegate)? { get set }
```

## Discussion

You can use a delegate object to provide the layer’s contents, handle the layout of any sublayers, and provide custom actions in response to layer-related changes. The object you assign to this property should implement one or more of the methods of the CALayerDelegate informal protocol. For more information about that protocol, see `CALayerDelegate`

In iOS, if the layer is associated with a UIView object, this property *must* be set to the view that owns the layer.

