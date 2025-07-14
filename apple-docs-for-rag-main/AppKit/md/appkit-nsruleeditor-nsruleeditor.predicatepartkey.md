

- AppKit
- NSRuleEditor
-  NSRuleEditor.PredicatePartKey 

Structure

# NSRuleEditor.PredicatePartKey

These strings are used as keys to the dictionary returned from the delegate’s ruleEditor(_:predicatePartsForCriterion:withDisplayValue:inRow:) optional method. To construct a valid predicate, the union of the dictionaries for each item in the row must contain the required parts.

macOS

``` source
struct PredicatePartKey
```

## Topics

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

static let options: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSNumber` object representing a NSComparisonPredicate_Optionsbitfield.

static let rightExpression: NSRuleEditor.PredicatePartKey

The corresponding value is an `NSExpression` object representing the right expression in the predicate.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Providing Data

func ruleEditor(NSRuleEditor, child: Int, forCriterion: Any?, with: NSRuleEditor.RowType) -> Any

Returns the child of a given item at a given index.

**Required**

func ruleEditor(NSRuleEditor, displayValueForCriterion: Any, inRow: Int) -> Any

Returns the value for a given criterion.

**Required**

func ruleEditor(NSRuleEditor, numberOfChildrenForCriterion: Any?, with: NSRuleEditor.RowType) -> Int

Returns the number of child items of a given criterion or row type.

**Required**

func ruleEditor(NSRuleEditor, predicatePartsForCriterion: Any, withDisplayValue: Any, inRow: Int) -> [NSRuleEditor.PredicatePartKey : Any]?

Returns a dictionary representing the parts of the predicate determined by the given criterion and value.

