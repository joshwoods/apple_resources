

- AppKit
- NSRuleEditorDelegate
-  ruleEditor(\_:displayValueForCriterion:inRow:) 

Instance Method

# ruleEditor(\_:displayValueForCriterion:inRow:)

Returns the value for a given criterion.

macOS

``` source
@MainActor
func ruleEditor(
    _ editor: NSRuleEditor,
    displayValueForCriterion criterion: Any,
    inRow row: Int
) -> Any
```

**Required**

## Parameters 

`editor`  

The rule editor that sent the message.

`criterion`  

The criterion for which the value is required.

`row`  

The row number of `criterion`.

## Return Value

The value for `criterion`.

## Discussion

The value should be an instance of `NSString`, `NSView`, or `NSMenuItem`. If the value is an `NSView` or `NSMenuItem`, you must ensure it is unique for every invocation of this method; that is, do not return a particular instance of `NSView` or `NSMenuItem` more than once.

### Special Considerations

The delegate must implement this method.

## See Also

### Providing Data

func ruleEditor(NSRuleEditor, child: Int, forCriterion: Any?, with: NSRuleEditor.RowType) -> Any

Returns the child of a given item at a given index.

**Required**

func ruleEditor(NSRuleEditor, numberOfChildrenForCriterion: Any?, with: NSRuleEditor.RowType) -> Int

Returns the number of child items of a given criterion or row type.

**Required**

func ruleEditor(NSRuleEditor, predicatePartsForCriterion: Any, withDisplayValue: Any, inRow: Int) -> [NSRuleEditor.PredicatePartKey : Any]?

Returns a dictionary representing the parts of the predicate determined by the given criterion and value.

struct PredicatePartKey

These strings are used as keys to the dictionary returned from the delegate’s ruleEditor(_:predicatePartsForCriterion:withDisplayValue:inRow:) optional method. To construct a valid predicate, the union of the dictionaries for each item in the row must contain the required parts.

