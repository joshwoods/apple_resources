

- Core Animation
- CALayer
-  constraints 

Instance Property

# constraints

The constraints used to position current layer’s sublayers.

Mac CatalystmacOS

``` source
var constraints: [CAConstraint]? { get set }
```

## Discussion

macOS apps can use this property to access their layer-based constraints. Before constraints can be applied, you must also assign a CAConstraintLayoutManager object to the layoutManager property of the layer.

iOS apps do not support layer-based constraints.

## See Also

### Managing Layer Constraints

func addConstraint(CAConstraint)

Adds the specified constraint to the layer.

