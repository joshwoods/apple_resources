

- AppKit
- NSPredicateEditorRowTemplate
-  setPredicate(\_:) 

Instance Method

# setPredicate(\_:)

Sets the value of the views according to the given predicate.

macOS 10.5+

``` source
func setPredicate(_ predicate: NSPredicate)
```

## Parameters 

`predicate`  

The predicate value for the receiver.

## Discussion

This method is only called if match(for:) returned a positive value for the receiver.

You can override this to set the values of custom views.

## See Also

### Primitive Methods

func match(for: NSPredicate) -> Double

Returns a positive number if the receiver can represent a given predicate, and `0` if it cannot.

var templateViews: [NSView]

Returns the views that display this template’s predicate.

func displayableSubpredicates(of: NSPredicate) -> [NSPredicate]?

Returns the subpredicates that should be made sub-rows of a given predicate.

func predicate(withSubpredicates: [NSPredicate]?) -> NSPredicate

Returns the predicate represented by the receiver’s views’ values and the given sub-predicates.

