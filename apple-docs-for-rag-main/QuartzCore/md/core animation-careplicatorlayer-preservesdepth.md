

- Core Animation
- CAReplicatorLayer
-  preservesDepth 

Instance Property

# preservesDepth

Defines whether this layer flattens its sublayers into its plane.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var preservesDepth: Bool { get set }
```

## Discussion

If true, the layer acts similarly to the `CATransformLayer` and has the same restrictions.

Default is false.

