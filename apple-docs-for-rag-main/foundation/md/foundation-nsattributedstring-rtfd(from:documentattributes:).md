

- Foundation
- NSAttributedString
-  rtfd(from:documentAttributes:) 

Instance Method

# rtfd(from:documentAttributes:)

Returns a data object that contains an RTFD stream corresponding to the characters and attributes within the specified range.

macOS 10.0+

``` source
func rtfd(
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

A data object containing the RTFD stream containing the characters and attributes.

## Discussion

Writes the document-level attributes in `docAttributes`, as explained in RTF Files and Attributed Strings.

Raises an rangeException if any part of `aRange` lies beyond the end of the receiver’s characters.

When writing data to the pasteboard, you can use the `NSData` object as the first argument to the NSPasteboard method setData(_:forType:), with a second argument of `NSRTFPboardType`.

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

func rtfdFileWrapper(from: NSRange, documentAttributes: [NSAttributedString.DocumentAttributeKey : Any]) -> FileWrapper?

Returns a file wrapper object that contains an RTFD document corresponding to the characters and attributes within the specified range.

