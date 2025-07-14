

- AppKit
-  NSRuleEditorDelegate 

Protocol

# NSRuleEditorDelegate

The `NSRuleEditorDelegate` protocol defines the optional methods implemented by delegates of NSRuleEditor objects.

macOS

``` source
protocol NSRuleEditorDelegate : NSObjectProtocol
```

## Topics

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

struct PredicatePartKey

These strings are used as keys to the dictionary returned from the delegate’s ruleEditor(_:predicatePartsForCriterion:withDisplayValue:inRow:) optional method. To construct a valid predicate, the union of the dictionaries for each item in the row must contain the required parts.

### Monitoring Row Changes

func ruleEditorRowsDidChange(Notification)

Notifies the receiver that a rule editor’s rows changed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Configuring the Delegate

var delegate: (any NSRuleEditorDelegate)?

The rule editor’s delegate.

