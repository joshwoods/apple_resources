

- Foundation
- XMLDocument
-  init(contentsOf:options:) 

Initializer

# init(contentsOf:options:)

Initializes and returns an NSXMLDocument object created from the XML or HTML contents of a URL-referenced source

Mac Catalyst 13.0+macOS 10.0+

``` source
convenience init(
    contentsOf url: URL,
    options mask: XMLNode.Options = []
) throws
```

## Parameters 

`url`  

An NSURL object specifying a URL source.

`mask`  

A bit mask for input options. You can specify multiple options by bit-OR’ing them. See Constants for a list of valid input options.

## Return Value

An initialized `NSXMLDocument` object, or `nil` if initialization fails because of parsing errors or other reasons.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

Tree-Based XML Programming Guide

### Initializing NSXMLDocument Objects

init(data: Data, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDocument` object created from an NSData object.

init(rootElement: XMLElement?)

Returns an `NSXMLDocument` object initialized with a single child, the root element.

convenience init(xmlString: String, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDocument` object created from a string containing XML markup text.

class func replacementClass(for: AnyClass) -> AnyClass

Overridden by subclasses to substitute a custom class for an NSXML class that the parser uses to create node instances.

