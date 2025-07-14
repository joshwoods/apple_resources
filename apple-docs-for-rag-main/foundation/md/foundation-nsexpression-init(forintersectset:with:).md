

- Foundation
- NSExpression
-  init(forIntersectSet:with:) 

Initializer

# init(forIntersectSet:with:)

Creates an expression object that represents the intersection of a specified set and collection.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    forIntersectSet left: NSExpression,
    with right: NSExpression
)
```

## Parameters 

`left`  

An expression that evaluates to an `NSSet` object.

`right`  

An expression that evaluates to a collection object (an instance of `NSArray`, `NSSet`, or `NSDictionary`).

## Return Value

A new `NSExpression` object that represents the intersection of `left` and `right`.

## See Also

### Creating a Collection Expression

init(forAggregate: [NSExpression])

Creates an aggregate expression for a specified collection.

init(forUnionSet: NSExpression, with: NSExpression)

Creates an expression object that represents the union of a specified set and collection.

init(forMinusSet: NSExpression, with: NSExpression)

Creates an expression object that represents the subtraction of a specified collection from a specified set.

