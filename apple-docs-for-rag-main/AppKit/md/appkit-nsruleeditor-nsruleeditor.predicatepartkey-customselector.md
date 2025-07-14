

- AppKit
- NSRuleEditor
- NSRuleEditor.PredicatePartKey
-  customSelector 

Type Property

# customSelector

The corresponding value is an `NSString` object representing a custom selector.

macOS

``` source
static let customSelector: NSRuleEditor.PredicatePartKey
```

## Discussion

If specified, this overrides the operator type, options, and comparison modifier.

## See Also

### Predicate Part Keys

static let comparisonModifier: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate.Modifier constant the of the predicate.

static let compoundType: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSCompoundPredicate.LogicalType constant.

static let leftExpression: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSExpression` object representing the left expression in the predicate.

static let operatorType: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate.Operator constant.

static let options: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate_Optionsbitfield.

static let rightExpression: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSExpression` object representing the right expression in the predicate.

