

- Foundation
- XMLDocument
-  validate() 

Instance Method

# validate()

Validates the document against the governing schema and returns whether the document conforms to the schema.

Mac Catalyst 13.0+macOS 10.0+

``` source
func validate() throws
```

## Discussion

The constants indicating the kind of validation errors are emitted by the underlying parser; see `NSXMLParser.h` for most of these constants. If the schema is defined with a DTD, this method uses the XMLDTD object set for the receiver for validation. If the schema is based on XML Schema, the method uses the URL specified as the value of the `xsi:schemaLocation` attribute of the root element.

You can validate an XML document when it is first processed by specifying the `NSXMLDocumentValidate` option when you initialize an `NSXMLDocument` object with the init(contentsOf:options:), init(data:options:), or init(xmlString:options:) methods.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

