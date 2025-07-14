

- AppKit
- NSRuleEditor
-  predicate 

Instance Property

# predicate

The rule editor’s predicate.

macOS

``` source
@MainActor
var predicate: NSPredicate? { get }
```

## Discussion

If the delegate implements NSRuleEditor, this property contains the rule editor’s predicate. If the delegate does not implement NSRuleEditor, or if the delegate does not return enough parts to construct a full predicate, this property contains `nil`.

## See Also

### Working with Predicates

func reloadPredicate()

Instructs the receiver to regenerate its predicate by invoking the corresponding delegate method.

func predicate(forRow: Int) -> NSPredicate?

Returns the predicate for a given row.

