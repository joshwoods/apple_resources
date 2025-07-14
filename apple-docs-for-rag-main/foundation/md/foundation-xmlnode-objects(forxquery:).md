

- Foundation
- XMLNode
-  objects(forXQuery:) 

Instance Method

# objects(forXQuery:)

Returns the objects resulting from executing an XQuery query upon the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func objects(forXQuery xquery: String) throws -> [Any]
```

## Parameters 

`xquery`  

A string that expresses an XQuery query.

## Discussion

The receiver acts as the context item for the query (”.”). If the receiver has been changed after parsing to have multiple adjacent text nodes, you should invoke the `NSXMLElement` method normalizeAdjacentTextNodesPreservingCDATA(_:) (with an argument of false) to coalesce the text nodes before querying .This convenience method invokes objects(forXQuery:constants:) with `nil` for the `constants` dictionary.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Executing Queries

func nodes(forXPath: String) throws -> [XMLNode]

Returns the nodes resulting from executing an XPath query upon the receiver.

func objects(forXQuery: String, constants: [String : Any]?) throws -> [Any]

Returns the objects resulting from executing an XQuery query upon the receiver.

var xPath: String?

Returns the XPath expression identifying the receiver’s location in the document tree.

