

- Core Animation
- CALayer
-  addConstraint(\_:) 

Instance Method

# addConstraint(\_:)

Adds the specified constraint to the layer.

Mac CatalystmacOS

``` source
func addConstraint(_ c: CAConstraint)
```

## Parameters 

`c`  

The constraint object to add to the receiver’s array of constraint objects.

## Discussion

In macOS, you typically add constraints to a layer to manage the size and position of that layer’s sublayers. Before constraints can be applied, you must also assign a CAConstraintLayoutManager object to the layoutManager property of the layer. For more information about managing layer-based constraints, see Core Animation Programming Guide.

iOS apps do not support layer-based constraints.

## See Also

### Managing Layer Constraints

var constraints: [CAConstraint]?

The constraints used to position current layer’s sublayers.

