

- Foundation
- XMLNode
-  nodes(forXPath:) 

Instance Method

# nodes(forXPath:)

Returns the nodes resulting from executing an XPath query upon the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func nodes(forXPath xpath: String) throws -> [XMLNode]
```

## Parameters 

`xpath`  

A string that expresses an XPath query.

## Return Value

An array of `NSXMLNode` objects that match the query, or an empty array if there are no matches.

## Discussion

The receiver acts as the context item for the query (”.”). If you have explicitly added adjacent text nodes as children of an element, you should invoke the `NSXMLElement` method normalizeAdjacentTextNodesPreservingCDATA(_:) (with an argument of false) on the element before applying any XPath queries to it; this method coalesces these text nodes. The same precaution applies if you have processed a document preserving CDATA sections and these sections are adjacent to text nodes.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Executing Queries

func objects(forXQuery: String) throws -> [Any]

Returns the objects resulting from executing an XQuery query upon the receiver.

func objects(forXQuery: String, constants: [String : Any]?) throws -> [Any]

Returns the objects resulting from executing an XQuery query upon the receiver.

var xPath: String?

Returns the XPath expression identifying the receiver’s location in the document tree.

