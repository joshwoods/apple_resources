

- AppKit
- NSPredicateEditorRowTemplate
-  init(leftExpressions:rightExpressionAttributeType:modifier:operators:options:) 

Initializer

# init(leftExpressions:rightExpressionAttributeType:modifier:operators:options:)

Initializes and returns a “pop-up-pop-up-view”–style row template.

macOS 10.5+

``` source
init(
    leftExpressions: [NSExpression],
    rightExpressionAttributeType attributeType: NSAttributeType,
    modifier: NSComparisonPredicate.Modifier,
    operators: [NSNumber],
    options: Int
)
```

## Parameters 

`leftExpressions`  

An array of NSExpression objects that represent the left side of a predicate.

`attributeType`  

An attribute type for the right side of a predicate. This value dictates the type of view created, and how the control’s object value is coerced before putting it into a predicate.

`modifier`  

A modifier for the predicate (see NSComparisonPredicate.Modifier for possible values).

`operators`  

An array of NSNumber objects specifying the operator type (see NSComparisonPredicate.Operator for possible values).

`options`  

Options for the predicate (see NSComparisonPredicate.Options for possible values).

## Return Value

A row template initialized using the specified arguments.

## Discussion

The type of `attributeType` dictates the type of view created. For example, NSAttributeType.dateAttributeType creates an NSDatePicker object, NSAttributeType.integer64AttributeType creates a short text field, and NSAttributeType.stringAttributeType produces a longer text field. You can resize the views as you want.

Predicates do not automatically coerce types for you. For example, comparing a number to a string will raise an exception. Therefore, the attribute type is also needed to determine how the control’s object value must be coerced before putting it into a predicate.

## See Also

### Initializing a Template

init(leftExpressions: [NSExpression], rightExpressions: [NSExpression], modifier: NSComparisonPredicate.Modifier, operators: [NSNumber], options: Int)

Initializes and returns a “pop-up-pop-up-pop-up”–style row template.

init(compoundTypes: [NSNumber])

Initializes and returns a row template suitable for displaying compound predicates.

