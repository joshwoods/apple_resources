

- Foundation
- NSComparisonPredicate
-  init(leftExpression:rightExpression:customSelector:) 

Initializer

# init(leftExpression:rightExpression:customSelector:)

Creates a predicate that you form by combining specified left and right expressions using a specified selector.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    leftExpression lhs: NSExpression,
    rightExpression rhs: NSExpression,
    customSelector selector: Selector
)
```

## Parameters 

`lhs`  

The left hand expression.

`rhs`  

The right hand expression.

`selector`  

The selector to use. The method defined by the selector must take a single argument and return a `BOOL` value.

## Return Value

The receiver, initialized by combining the left and right expressions using `selector`.

## See Also

### Creating Comparison Predicates

Displaying searchable content by using a search controller

Create a user interface with searchable content in a table view.

init(leftExpression: NSExpression, rightExpression: NSExpression, modifier: NSComparisonPredicate.Modifier, type: NSComparisonPredicate.Operator, options: NSComparisonPredicate.Options)

Creates a predicate to a specified type that you form by combining specified left and right expressions using a specified modifier and options.

init?(coder: NSCoder)

Creates a predicate by decoding from the coder you specify.

