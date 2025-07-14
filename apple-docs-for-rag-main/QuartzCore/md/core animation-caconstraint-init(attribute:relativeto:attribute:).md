

- Core Animation
- CAConstraint
-  init(attribute:relativeTo:attribute:) 

Initializer

# init(attribute:relativeTo:attribute:)

Creates and returns an `CAConstraint` object with the specified parameters.

Mac Catalyst 13.1+macOS 10.5+

``` source
convenience init(
    attribute attr: CAConstraintAttribute,
    relativeTo srcId: String,
    attribute srcAttr: CAConstraintAttribute
)
```

## Parameters 

`attr`  

The attribute of the layer for which to create a new constraint.

`srcId`  

The name of the layer that this constraint is calculated relative to.

`srcAttr`  

The attribute of `srcLayer` the constraint is calculated relative to.

## Return Value

A new `CAConstraint` object with the specified parameters. The scale of the constraint is set to 1.0. The offset of the constraint is set to 0.0.

## Discussion

The value for the constraint is calculated is `srcAttr`.

## See Also

### Create a New Constraint

convenience init(attribute: CAConstraintAttribute, relativeTo: String, attribute: CAConstraintAttribute, offset: CGFloat)

Creates and returns an `CAConstraint` object with the specified parameters.

init(attribute: CAConstraintAttribute, relativeTo: String, attribute: CAConstraintAttribute, scale: CGFloat, offset: CGFloat)

Returns an `CAConstraint` object with the specified parameters. Designated initializer.

