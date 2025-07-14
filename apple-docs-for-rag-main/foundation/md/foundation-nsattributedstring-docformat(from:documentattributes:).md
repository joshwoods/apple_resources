

- Foundation
- NSAttributedString
-  docFormat(from:documentAttributes:) 

Instance Method

# docFormat(from:documentAttributes:)

Returns a data object that contains a Microsoft Word–format stream corresponding to the characters and attributes within the specified range.

macOS 10.0+

``` source
func docFormat(
    from range: NSRange,
    documentAttributes dict: [NSAttributedString.DocumentAttributeKey : Any] = [:]
) -> Data?
```

## Parameters 

`range`  

The range.

`dict`  

A required dictionary specifying the document attributes. The dictionary contains values from `Document Types` and must at least contain documentType.

## Return Value

Returns a data object containing the attributed string as a Microsoft Word doc file.

## Discussion

Raises an rangeException if any part of `range` lies beyond the end of the receiver’s characters.

## See Also

### Exporting the string as data

func data(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) throws -> Data

Returns a data object that contains a text stream corresponding to the characters and attributes within the specified range.

func fileWrapper(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) throws -> FileWrapper

Returns a file wrapper object that contains a text stream corresponding to the characters and attributes within the specified range.

func rtf(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> Data?

Returns a data object that contains an RTF stream corresponding to the characters and attributes within the specified range, omitting all attachment attributes.

func rtfd(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> Data?

Returns a data object that contains an RTFD stream corresponding to the characters and attributes within the specified range.

func rtfdFileWrapper(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> FileWrapper?

Returns a file wrapper object that contains an RTFD document corresponding to the characters and attributes within the specified range.

