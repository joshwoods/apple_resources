

- Foundation
- NSComparisonPredicate
-  init(coder:) 

Initializer

# init(coder:)

Creates a predicate by decoding from the coder you specify.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(coder: NSCoder)
```

## Parameters 

`coder`  

The coder to read data from.

## See Also

### Creating Comparison Predicates

Displaying searchable content by using a search controller

Create a user interface with searchable content in a table view.

init(leftExpression: NSExpression, rightExpression: NSExpression, customSelector: Selector)

Creates a predicate that you form by combining specified left and right expressions using a specified selector.

init(leftExpression: NSExpression, rightExpression: NSExpression, modifier: NSComparisonPredicate.Modifier, type: NSComparisonPredicate.Operator, options: NSComparisonPredicate.Options)

Creates a predicate to a specified type that you form by combining specified left and right expressions using a specified modifier and options.

