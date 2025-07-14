

- Foundation
- XMLElement
-  init(xmlString:) 

Initializer

# init(xmlString:)

Returns an `NSXMLElement` object created from a specified string containing XML markup.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(xmlString string: String) throws
```

## Parameters 

`string`  

A string containing XML markup for an element.

## Return Value

The initialized `NSXMLElement` object or `nil` if initialization did not succeed.

## Discussion

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Initializing NSXMLElement Objects

convenience init(name: String)

Returns an `NSXMLElement` object initialized with the specified name.

convenience init(name: String, stringValue: String?)

Returns an `NSXMLElement` object initialized with a specified name and a single text-node child containing a specified value.

init(name: String, uri: String?)

Returns an `NSXMLElement` object initialized with the specified name and URI.

convenience init(kind: XMLNode.Kind, options: XMLNode.Options)

