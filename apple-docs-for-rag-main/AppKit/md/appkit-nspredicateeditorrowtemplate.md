

- AppKit
-  NSPredicateEditorRowTemplate 

Class

# NSPredicateEditorRowTemplate

A template that describes available predicates and how to display them.

macOS 10.5+

``` source
class NSPredicateEditorRowTemplate
```

## Overview

You can create instances of `NSPredicateEditorRowTemplate` programmatically or in Interface Builder. By default, a noncompound row template has three views: a popup (or static text field) on the left, a popup or static text field for operators, and either a popup or other view on the right.  You can subclass `NSPredicateEditorRowTemplate` to create a row template with different numbers or types of views.

`NSPredicateEditorRowTemplate` is a concrete class, but it has five primitive methods that are called by NSPredicateEditor: templateViews, match(for:), setPredicate(_:), displayableSubpredicates(of:), and predicate(withSubpredicates:). `NSPredicateEditorRowTemplate` implements all of these methods, but you can override them for custom templates. The primitive methods are used by an instance of `NSPredicateEditor` as follows.

First, an instance of `NSPredicateEditor` is created, and some row templates are set on it—either through a nib file or programmatically. The first thing predicate editor does is ask each of the templates for their views, using templateViews.

After setting up the predicate editor, you typically send it a objectValue message to restore a saved predicate. `NSPredicateEditor` needs to determine which of its templates should display each predicate in the predicate tree. It does this by sending each of its row templates a match(for:) message and choosing the one that returns the highest value.

After finding the best match for a predicate, `NSPredicateEditor` copies that template to get fresh views, inserts them into the proper row, and then sets the predicate on the template using setPredicate(_:). Within that method, the `NSPredicateEditorRowTemplate` object must set its views’ values to represent that predicate.

`NSPredicateEditorRowTemplate` next asks the template for the “displayable sub-predicates” of the predicate by sending a displayableSubpredicates(of:) message. If a template represents a predicate in its entirety, or if the predicate has no subpredicates, it can return `nil` for this.  Otherwise, it should return a list of predicates to be made into sub-rows of that template’s row. The whole process repeats for each sub-predicate.

At this point, the user sees the predicate that was saved.  If the user then makes some changes to the views of the templates, this causes `NSPredicateEditor` to recompute its predicate by asking each of the templates to return the predicate represented by the new view values, passing in the subpredicates represented by the sub-rows (an empty array if there are none, or `nil` if they aren’t supported by that predicate type):

predicate(withSubpredicates:)

## Topics

### Initializing a Template

init(leftExpressions: [NSExpression], rightExpressions: [NSExpression], modifier: NSComparisonPredicate.Modifier, operators: [NSNumber], options: Int)

Initializes and returns a “pop-up-pop-up-pop-up”–style row template.

init(leftExpressions: [NSExpression], rightExpressionAttributeType: NSAttributeType, modifier: NSComparisonPredicate.Modifier, operators: [NSNumber], options: Int)

Initializes and returns a “pop-up-pop-up-view”–style row template.

init(compoundTypes: [NSNumber])

Initializes and returns a row template suitable for displaying compound predicates.

### Core Data Integration

class func templates(withAttributeKeyPaths: [String], in: NSEntityDescription) -> [NSPredicateEditorRowTemplate]

Returns an array of predicate templates for the given attribute key paths for a given entity.

### Primitive Methods

func match(for: NSPredicate) -> Double

Returns a positive number if the receiver can represent a given predicate, and `0` if it cannot.

var templateViews: [NSView]

Returns the views that display this template’s predicate.

func setPredicate(NSPredicate)

Sets the value of the views according to the given predicate.

func displayableSubpredicates(of: NSPredicate) -> [NSPredicate]?

Returns the subpredicates that should be made sub-rows of a given predicate.

func predicate(withSubpredicates: [NSPredicate]?) -> NSPredicate

Returns the predicate represented by the receiver’s views’ values and the given sub-predicates.

### Information About a Row Template

var leftExpressions: [NSExpression]?

Returns the left hand expressions for the receiver.

var rightExpressions: [NSExpression]?

Returns the right hand expressions for the receiver.

var compoundTypes: [NSNumber]?

Returns the compound predicate types.

var modifier: NSComparisonPredicate.Modifier

Returns the comparison predicate modifier for the receiver.

var operators: [NSNumber]?

Returns the array of comparison predicate operators.

var options: Int

Returns the comparison predicate options.

var rightExpressionAttributeType: NSAttributeType

Returns the attribute type of the receiver’s right expression.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Managing Row Templates

var rowTemplates: [NSPredicateEditorRowTemplate]

The row templates for the receiver.

