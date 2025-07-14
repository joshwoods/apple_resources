

- AppKit
- NSRuleEditor
- NSRuleEditor.PredicatePartKey
-  operatorType 

Type Property

# operatorType

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate.Operator constant.

macOS

``` source
static let operatorType: NSRuleEditor.PredicatePartKey
```

## Discussion

This value is required for a non-`nil` comparison predicate.

## See Also

### Predicate Part Keys

static let comparisonModifier: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate.Modifier constant the of the predicate.

static let compoundType: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSCompoundPredicate.LogicalType constant.

static let customSelector: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSString` object representing a custom selector.

static let leftExpression: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSExpression` object representing the left expression in the predicate.

static let options: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate_Optionsbitfield.

static let rightExpression: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSExpression` object representing the right expression in the predicate.

