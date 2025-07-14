

- AppKit
- NSPredicateEditorRowTemplate
-  predicate(withSubpredicates:) 

Instance Method

# predicate(withSubpredicates:)

Returns the predicate represented by the receiver’s views’ values and the given sub-predicates.

macOS 10.5+

``` source
func predicate(withSubpredicates subpredicates: [NSPredicate]?) -> NSPredicate
```

## Parameters 

`subpredicates`  

An array of predicates.

## Return Value

The predicate represented by the values of the template’s views and the given subpredicates. You can override this method to return the predicate represented by your custom views.

## Discussion

This method is only called if match(for:) returned a positive value for the receiver.

You can override this method to return the predicate represented by a custom view.

## See Also

### Primitive Methods

func match(for: NSPredicate) -> Double

Returns a positive number if the receiver can represent a given predicate, and `0` if it cannot.

var templateViews: [NSView]

Returns the views that display this template’s predicate.

func setPredicate(NSPredicate)

Sets the value of the views according to the given predicate.

func displayableSubpredicates(of: NSPredicate) -> [NSPredicate]?

Returns the subpredicates that should be made sub-rows of a given predicate.

