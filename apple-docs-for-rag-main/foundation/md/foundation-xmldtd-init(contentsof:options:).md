

- Foundation
- XMLDTD
-  init(contentsOf:options:) 

Initializer

# init(contentsOf:options:)

Initializes and returns an `NSXMLDTD` object created from the DTD declarations in a URL-referenced source.

Mac Catalyst 13.0+macOS 10.0+

``` source
convenience init(
    contentsOf url: URL,
    options mask: XMLNode.Options = []
) throws
```

## Parameters 

`url`  

An NSURL object identifying a URL source.

`mask`  

A bit mask specifying input options; bit-OR multiple options. The current valid options are `NSXMLNodePreserveWhitespace` and `NSXMLNodePreserveEntities`; these constants are described in the “Constants” section of the XMLNode reference.

## Return Value

An initialized `NSXMLDTD` object or `nil` if initialization fails because of parsing errors or other reasons.

## Discussion

You use this method to create a stand-alone DTD which you can thereafter query and use for validation. You can associate the DTD created through this message with a document by setting the dtd property on an XMLDocument object.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func validate() throws

Validates the document against the governing schema and returns whether the document conforms to the schema.

Tree-Based XML Programming Guide

### Initializing an NSXMLDTD Object

init(data: Data, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDTD` object created from the DTD declarations encapsulated in an NSData object

