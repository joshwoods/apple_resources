

- AppKit
- NSRuleEditor
- NSRuleEditor.PredicatePartKey
-  compoundType 

Type Property

# compoundType

The corresponding value is an `NSNumber` object representing a NSCompoundPredicate.LogicalType constant.

macOS

``` source
static let compoundType: NSRuleEditor.PredicatePartKey
```

## Discussion

If specified, the other keys are ignored and the predicate for the row will be an `NSCompoundPredicate` predicate whose subpredicates are the predicates of the subrows of the given row.

## See Also

### Predicate Part Keys

static let comparisonModifier: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate.Modifier constant the of the predicate.

static let customSelector: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSString` object representing a custom selector.

static let leftExpression: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSExpression` object representing the left expression in the predicate.

static let operatorType: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate.Operator constant.

static let options: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate_Optionsbitfield.

static let rightExpression: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSExpression` object representing the right expression in the predicate.

