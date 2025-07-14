

- Foundation
- NSAttributedString
-  init(RTF:documentAttributes:) 

Initializer

# init(RTF:documentAttributes:)

Creates an attributed string by decoding the stream of RTF commands and data in the specified data object.

macOS 10.0+

``` source
init?(
    RTF data: Data,
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
)
```

``` source
init?(
    rtf data: Data,
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
)
```

## Parameters 

`data`  

The data containing RTF content.

`dict`  

An in-out dictionary containing document-level attributes. On output, this method updates the dictionary to contain any document-specific keys found in the data. Specify `nil` if you don’t want the document attributes.

## Return Value

Returns an initialized attributed string object, or `nil` if the method can’t decode the data.

## Discussion

Also returns by reference in `dict` a dictionary containing document-level attributes described in NSAttributedString.DocumentAttributeKey. `dict` may be `NULL`, in which case no document attributes are returned. Returns an initialized object, or `nil` if `data` can’t be decoded.

## See Also

### Creating from RTF

init?(RTFD: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string by decoding the stream of RTFD commands and data in the specified data object.

init?(RTFDFileWrapper: FileWrapper, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from the specified file wrapper that contains an RTFD document.

