

- Foundation
- XMLDTD
-  init(data:options:) 

Initializer

# init(data:options:)

Initializes and returns an `NSXMLDTD` object created from the DTD declarations encapsulated in an NSData object

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    data: Data,
    options mask: XMLNode.Options = []
) throws
```

## Parameters 

`data`  

A data object containing DTD declarations.

`mask`  

A bit mask specifying input options; bit-OR multiple options. The current valid options are `NSXMLNodePreserveWhitespace` and `NSXMLNodePreserveEntities`; these constants are described in the “Constants” section of the XMLNode reference.

## Return Value

An initialized `NSXMLDTD` object or `nil` if initialization fails because of parsing errors or other reasons.

## Discussion

This method is the designated initializer for the `NSXMLDTD` class. You use this method to create a stand-alone DTD which you can thereafter query and use for validation. You can associate the DTD created through this message with a document by setting the dtd property on an XMLDocument object.

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func validate() throws

Validates the document against the governing schema and returns whether the document conforms to the schema.

### Initializing an NSXMLDTD Object

convenience init(contentsOf: URL, options: XMLNode.Options) throws

Initializes and returns an `NSXMLDTD` object created from the DTD declarations in a URL-referenced source.

