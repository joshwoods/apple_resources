

- AppKit
- NSPredicateEditorRowTemplate
-  templateViews 

Instance Property

# templateViews

Returns the views that display this template’s predicate.

macOS 10.5+

``` source
var templateViews: [NSView] { get }
```

## Return Value

The views for an NSPredicateEditor to display in a row that represents the predicate from setPredicate(_:).

## Discussion

NSPredicateEditor treats instances of NSPopUpButton specially by merging their menu items into a single popup button, and by combining menu items with matching titles. In this way, the editor builds a single tree from the separate templates.

## See Also

### Primitive Methods

func match(for: NSPredicate) -> Double

Returns a positive number if the receiver can represent a given predicate, and `0` if it cannot.

func setPredicate(NSPredicate)

Sets the value of the views according to the given predicate.

func displayableSubpredicates(of: NSPredicate) -> [NSPredicate]?

Returns the subpredicates that should be made sub-rows of a given predicate.

func predicate(withSubpredicates: [NSPredicate]?) -> NSPredicate

Returns the predicate represented by the receiver’s views’ values and the given sub-predicates.

