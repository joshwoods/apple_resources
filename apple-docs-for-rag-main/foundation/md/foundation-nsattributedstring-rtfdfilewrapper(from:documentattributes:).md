

- Foundation
- NSAttributedString
-  rtfdFileWrapper(from:documentAttributes:) 

Instance Method

# rtfdFileWrapper(from:documentAttributes:)

Returns a file wrapper object that contains an RTFD document corresponding to the characters and attributes within the specified range.

macOS 10.0+

``` source
func rtfdFileWrapper(
    from range: NSRange,
    documentAttributes dict: [NSAttributedString.DocumentAttributeKey : Any] = [:]
) -> FileWrapper?
```

## Parameters 

`range`  

The range.

`dict`  

A required dictionary specifying the document attributes. The dictionary contains values from `Document Types` and must at least contain `NSDocumentTypeDocumentAttribute`.

## Return Value

A file wrapper containing the RTFD data.

## Discussion

The file wrapper also includes the document-level attributes in `docAttributes`, as explained in RTF Files and Attributed Strings.

Raises an rangeException if any part of `aRange` lies beyond the end of the receiver’s characters.

You can save the file wrapper using the write(toFile:atomically:updateFilenames:) method of FileWrapper.

## See Also

### Exporting the string as data

func data(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) throws -> Data

Returns a data object that contains a text stream corresponding to the characters and attributes within the specified range.

func fileWrapper(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) throws -> FileWrapper

Returns a file wrapper object that contains a text stream corresponding to the characters and attributes within the specified range.

func docFormat(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> Data?

Returns a data object that contains a Microsoft Word–format stream corresponding to the characters and attributes within the specified range.

func rtf(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> Data?

Returns a data object that contains an RTF stream corresponding to the characters and attributes within the specified range, omitting all attachment attributes.

func rtfd(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> Data?

Returns a data object that contains an RTFD stream corresponding to the characters and attributes within the specified range.

