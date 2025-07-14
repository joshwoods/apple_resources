

- AppKit
- NSPredicateEditorRowTemplate
-  init(compoundTypes:) 

Initializer

# init(compoundTypes:)

Initializes and returns a row template suitable for displaying compound predicates.

macOS 10.5+

``` source
init(compoundTypes: [NSNumber])
```

## Parameters 

`compoundTypes`  

An array of NSNumber objects specifying compound predicate types. See NSCompoundPredicate.LogicalType for possible values.

## Return Value

A row template initialized for displaying compound predicates of the types specified by `compoundTypes`.

## Discussion

NSPredicateEditor contains such a template by default.

## See Also

### Initializing a Template

init(leftExpressions: [NSExpression], rightExpressions: [NSExpression], modifier: NSComparisonPredicate.Modifier, operators: [NSNumber], options: Int)

Initializes and returns a “pop-up-pop-up-pop-up”–style row template.

init(leftExpressions: [NSExpression], rightExpressionAttributeType: NSAttributeType, modifier: NSComparisonPredicate.Modifier, operators: [NSNumber], options: Int)

Initializes and returns a “pop-up-pop-up-view”–style row template.

