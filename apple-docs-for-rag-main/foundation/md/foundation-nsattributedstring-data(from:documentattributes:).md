

- Foundation
- NSAttributedString
-  data(from:documentAttributes:) 

Instance Method

# data(from:documentAttributes:)

Returns a data object that contains a text stream corresponding to the characters and attributes within the specified range.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func data(
    from range: NSRange,
    documentAttributes dict: [NSAttributedString.DocumentAttributeKey : Any] = [:]
) throws -> Data
```

## Parameters 

`range`  

The range.

`dict`  

A required dictionary specifying the document attributes. The dictionary contains values from `Document Types` and must at least contain documentType.

## Return Value

Returns the data for the attributed string, or `nil` if failure. When `nil`, `error` encapsulates the error information.

## Discussion

Raises an rangeException if any part of `range` lies beyond the end of the receiver’s characters.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Exporting the string as data

func fileWrapper(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) throws -> FileWrapper

Returns a file wrapper object that contains a text stream corresponding to the characters and attributes within the specified range.

func docFormat(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> Data?

Returns a data object that contains a Microsoft Word–format stream corresponding to the characters and attributes within the specified range.

func rtf(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> Data?

Returns a data object that contains an RTF stream corresponding to the characters and attributes within the specified range, omitting all attachment attributes.

func rtfd(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> Data?

Returns a data object that contains an RTFD stream corresponding to the characters and attributes within the specified range.

func rtfdFileWrapper(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> FileWrapper?

Returns a file wrapper object that contains an RTFD document corresponding to the characters and attributes within the specified range.

