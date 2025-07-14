

- AppKit
- NSPredicateEditorRowTemplate
-  init(leftExpressions:rightExpressions:modifier:operators:options:) 

Initializer

# init(leftExpressions:rightExpressions:modifier:operators:options:)

Initializes and returns a “pop-up-pop-up-pop-up”–style row template.

macOS 10.5+

``` source
init(
    leftExpressions: [NSExpression],
    rightExpressions: [NSExpression],
    modifier: NSComparisonPredicate.Modifier,
    operators: [NSNumber],
    options: Int
)
```

## Parameters 

`leftExpressions`  

An array of NSExpression objects that represent the left side of a predicate.

`rightExpressions`  

An array of NSExpression objects that represent the right side of a predicate.

`modifier`  

A modifier for the predicate (see NSComparisonPredicate.Modifier for possible values).

`operators`  

An array of NSNumber objects specifying the operator type (see NSComparisonPredicate.Operator for possible values).

`options`  

Options for the predicate (see NSComparisonPredicate.Options for possible values).

## Return Value

A row template of the “pop-up-pop-up-pop-up” form, with the left and right pop-ups representing the left and right expression arrays `leftExpressions` and `rightExpressions`, and the center pop-up representing the operators.

## See Also

### Related Documentation

Predicate Programming Guide

Control and Cell Programming Topics

### Initializing a Template

init(leftExpressions: [NSExpression], rightExpressionAttributeType: NSAttributeType, modifier: NSComparisonPredicate.Modifier, operators: [NSNumber], options: Int)

Initializes and returns a “pop-up-pop-up-view”–style row template.

init(compoundTypes: [NSNumber])

Initializes and returns a row template suitable for displaying compound predicates.

