

- AppKit
- NSRuleEditor
-  reloadPredicate() 

Instance Method

# reloadPredicate()

Instructs the receiver to regenerate its predicate by invoking the corresponding delegate method.

macOS

``` source
@MainActor
func reloadPredicate()
```

## Discussion

You typically invoke this method because something has changed (for example, a view’s value).

## See Also

### Working with Predicates

var predicate: NSPredicate?

The rule editor’s predicate.

func predicate(forRow: Int) -> NSPredicate?

Returns the predicate for a given row.

