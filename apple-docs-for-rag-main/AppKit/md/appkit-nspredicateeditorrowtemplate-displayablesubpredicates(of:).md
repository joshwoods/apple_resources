

- AppKit
- NSPredicateEditorRowTemplate
-  displayableSubpredicates(of:) 

Instance Method

# displayableSubpredicates(of:)

Returns the subpredicates that should be made sub-rows of a given predicate.

macOS 10.5+

``` source
func displayableSubpredicates(of predicate: NSPredicate) -> [NSPredicate]?
```

## Parameters 

`predicate`  

A predicate object.

## Return Value

The subpredicates that should be made sub-rows of `predicate`. For compound predicates (instances of NSCompoundPredicate), the array of subpredicates; for other types of predicate, returns `nil`. If a template represents a predicate in its entirety, or if the predicate has no subpredicates, returns `nil`.

## Discussion

You can override this method to create custom templates that handle complicated compound predicates.

## See Also

### Primitive Methods

func match(for: NSPredicate) -> Double

Returns a positive number if the receiver can represent a given predicate, and `0` if it cannot.

var templateViews: [NSView]

Returns the views that display this template’s predicate.

func setPredicate(NSPredicate)

Sets the value of the views according to the given predicate.

func predicate(withSubpredicates: [NSPredicate]?) -> NSPredicate

Returns the predicate represented by the receiver’s views’ values and the given sub-predicates.

