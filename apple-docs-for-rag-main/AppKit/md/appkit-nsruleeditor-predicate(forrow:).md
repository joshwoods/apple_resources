

- AppKit
- NSRuleEditor
-  predicate(forRow:) 

Instance Method

# predicate(forRow:)

Returns the predicate for a given row.

macOS

``` source
@MainActor
func predicate(forRow row: Int) -> NSPredicate?
```

## Parameters 

`row`  

The index of a row in the receiver.

## Return Value

The predicate for the row at `row`.

## Discussion

You should rarely have a need to call this directly, but you can override this method in a subclass to perform specialized predicate handling for certain criteria or display values.

## See Also

### Working with Predicates

var predicate: NSPredicate?

The rule editor’s predicate.

func reloadPredicate()

Instructs the receiver to regenerate its predicate by invoking the corresponding delegate method.

