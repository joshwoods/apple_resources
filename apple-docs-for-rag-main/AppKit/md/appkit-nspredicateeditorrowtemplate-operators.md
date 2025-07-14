

- AppKit
- NSPredicateEditorRowTemplate
-  operators 

Instance Property

# operators

Returns the array of comparison predicate operators.

macOS 10.5+

``` source
var operators: [NSNumber]? { get }
```

## Return Value

The array of NSNumber objects specifying the comparison predicate operators. See NSComparisonPredicate.Operator for possible values.

## See Also

### Information About a Row Template

var leftExpressions: [NSExpression]?

Returns the left hand expressions for the receiver.

var rightExpressions: [NSExpression]?

Returns the right hand expressions for the receiver.

var compoundTypes: [NSNumber]?

Returns the compound predicate types.

var modifier: NSComparisonPredicate.Modifier

Returns the comparison predicate modifier for the receiver.

var options: Int

Returns the comparison predicate options.

var rightExpressionAttributeType: NSAttributeType

Returns the attribute type of the receiver’s right expression.

