

- AppKit
- NSRuleEditorDelegate
-  ruleEditor(\_:child:forCriterion:with:) 

Instance Method

# ruleEditor(\_:child:forCriterion:with:)

Returns the child of a given item at a given index.

macOS

``` source
@MainActor
func ruleEditor(
    _ editor: NSRuleEditor,
    child index: Int,
    forCriterion criterion: Any?,
    with rowType: NSRuleEditor.RowType
) -> Any
```

**Required**

## Parameters 

`editor`  

The rule editor that sent the message.

`index`  

The index of the requested child criterion. This value must be in the range from `0` up to (but not including) the number of children, as reported by the delegate in ruleEditor(_:numberOfChildrenForCriterion:with:).

`criterion`  

The parent of the requested child, or `nil` if the rule editor is requesting a root criterion.

`rowType`  

The type of the row.

## Return Value

An object representing the requested child (or root) criterion. This object is used by the delegate to represent that position in the tree, and is passed as a parameter in subsequent calls to the delegate.

## Discussion

The delegate must implement this method.

## See Also

### Related Documentation

Predicate Programming Guide

Control and Cell Programming Topics

### Providing Data

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

