

- AppKit
- NSRuleEditorDelegate
-  ruleEditor(\_:numberOfChildrenForCriterion:with:) 

Instance Method

# ruleEditor(\_:numberOfChildrenForCriterion:with:)

Returns the number of child items of a given criterion or row type.

macOS

``` source
@MainActor
func ruleEditor(
    _ editor: NSRuleEditor,
    numberOfChildrenForCriterion criterion: Any?,
    with rowType: NSRuleEditor.RowType
) -> Int
```

**Required**

## Parameters 

`editor`  

The rule editor that sent the message.

`criterion`  

The criterion for which the number of children is required.

`rowType`  

The type of row of `criterion`.

## Return Value

The number of child items of `criterion`. If `criterion` is `nil`, return the number of root criteria for the row type `rowType`.

## Discussion

The delegate must implement this method.

## See Also

### Providing Data

func ruleEditor(NSRuleEditor, child: Int, forCriterion: Any?, with: NSRuleEditor.RowType) -> Any

Returns the child of a given item at a given index.

**Required**

func ruleEditor(NSRuleEditor, displayValueForCriterion: Any, inRow: Int) -> Any

Returns the value for a given criterion.

**Required**

func ruleEditor(NSRuleEditor, predicatePartsForCriterion: Any, withDisplayValue: Any, inRow: Int) -> [NSRuleEditor.PredicatePartKey : Any]?

Returns a dictionary representing the parts of the predicate determined by the given criterion and value.

struct PredicatePartKey

These strings are used as keys to the dictionary returned from the delegate’s ruleEditor(_:predicatePartsForCriterion:withDisplayValue:inRow:) optional method. To construct a valid predicate, the union of the dictionaries for each item in the row must contain the required parts.

