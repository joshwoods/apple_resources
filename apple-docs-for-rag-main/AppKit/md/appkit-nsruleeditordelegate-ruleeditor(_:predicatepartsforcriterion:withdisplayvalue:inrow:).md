

- AppKit
- NSRuleEditorDelegate
-  ruleEditor(\_:predicatePartsForCriterion:withDisplayValue:inRow:) 

Instance Method

# ruleEditor(\_:predicatePartsForCriterion:withDisplayValue:inRow:)

Returns a dictionary representing the parts of the predicate determined by the given criterion and value.

macOS

``` source
@MainActor
optional func ruleEditor(
    _ editor: NSRuleEditor,
    predicatePartsForCriterion criterion: Any,
    withDisplayValue value: Any,
    inRow row: Int
) -> [NSRuleEditor.PredicatePartKey : Any]?
```

## Parameters 

`editor`  

The rule editor that sent the message.

`criterion`  

The criterion for which the predicate parts are required.

`value`  

The display value.

`row`  

The row number of `criterion`.

## Return Value

A dictionary representing the parts of the predicate determined by the given criterion and value. The keys of the dictionary should be the string constants specified in Predicate Part Keys with corresponding appropriate values.

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

struct PredicatePartKey

These strings are used as keys to the dictionary returned from the delegate’s ruleEditor(_:predicatePartsForCriterion:withDisplayValue:inRow:) optional method. To construct a valid predicate, the union of the dictionaries for each item in the row must contain the required parts.

