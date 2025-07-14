

- AppKit
- NSPredicateEditorRowTemplate
-  compoundTypes 

Instance Property

# compoundTypes

Returns the compound predicate types.

macOS 10.5+

``` source
var compoundTypes: [NSNumber]? { get }
```

## Return Value

An array of NSNumber objects specifying compound predicate types. See NSCompoundPredicate.LogicalType for possible values.

## See Also

### Information About a Row Template

var leftExpressions: [NSExpression]?

Returns the left hand expressions for the receiver.

var rightExpressions: [NSExpression]?

Returns the right hand expressions for the receiver.

var modifier: NSComparisonPredicate.Modifier

Returns the comparison predicate modifier for the receiver.

var operators: [NSNumber]?

Returns the array of comparison predicate operators.

var options: Int

Returns the comparison predicate options.

var rightExpressionAttributeType: NSAttributeType

Returns the attribute type of the receiver’s right expression.

