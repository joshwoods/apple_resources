

- AppKit
- NSRuleEditor
- NSRuleEditor.PredicatePartKey
-  options 

Type Property

# options

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate_Optionsbitfield.

macOS

``` source
static let options: NSRuleEditor.PredicatePartKey
```

## Discussion

If no value is specified, `0` (no options) is assumed.

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

static let operatorType: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate.Operator constant.

static let rightExpression: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSExpression` object representing the right expression in the predicate.

