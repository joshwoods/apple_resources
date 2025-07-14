

- Core Animation
- CAConstraint
-  init(attribute:relativeTo:attribute:scale:offset:) 

Initializer

# init(attribute:relativeTo:attribute:scale:offset:)

Returns an `CAConstraint` object with the specified parameters. Designated initializer.

Mac Catalyst 13.1+macOS 10.5+

``` source
init(
    attribute attr: CAConstraintAttribute,
    relativeTo srcId: String,
    attribute srcAttr: CAConstraintAttribute,
    scale m: CGFloat,
    offset c: CGFloat
)
```

## Parameters 

`attr`  

The attribute of the layer for which to create a new constraint.

`srcId`  

The name of the layer that this constraint is calculated relative to.

`srcAttr`  

The attribute of `srcLayer` the constraint is calculated relative to.

`m`  

The amount to scale the value of `srcAttr`.

`c`  

The offset added to the value of `srcAttr`.

## Return Value

An initialized constraint object using the specified parameters.

## Discussion

The value for the constraint is calculated as (`srcAttr` \* `scale`) + `offset`).

## See Also

### Create a New Constraint

convenience init(attribute: CAConstraintAttribute, relativeTo: String, attribute: CAConstraintAttribute, offset: CGFloat)

Creates and returns an `CAConstraint` object with the specified parameters.

convenience init(attribute: CAConstraintAttribute, relativeTo: String, attribute: CAConstraintAttribute)

Creates and returns an `CAConstraint` object with the specified parameters.

