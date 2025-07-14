

- AppKit
- NSPredicateEditorRowTemplate
-  options 

Instance Property

# options

Returns the comparison predicate options.

macOS 10.5+

``` source
var options: Int { get }
```

## Return Value

The comparison predicate options for the receiver. See NSComparisonPredicate.Options for possible values. Returns `0` if this does not apply (for example, for a compound template initialized with init(compoundTypes:)).

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

var operators: [NSNumber]?

Returns the array of comparison predicate operators.

var rightExpressionAttributeType: NSAttributeType

Returns the attribute type of the receiver’s right expression.

