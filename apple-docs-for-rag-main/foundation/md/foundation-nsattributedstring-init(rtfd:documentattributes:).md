

- Foundation
- NSAttributedString
-  init(RTFD:documentAttributes:) 

Initializer

# init(RTFD:documentAttributes:)

Creates an attributed string by decoding the stream of RTFD commands and data in the specified data object.

macOS 10.0+

``` source
init?(
    RTFD data: Data,
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
)
```

``` source
init?(
    rtfd data: Data,
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
)
```

## Parameters 

`data`  

The data containing the RTFD content.

`dict`  

An in-out dictionary containing document-level attributes. On output, this method updates the dictionary to contain any document-specific keys found in the data. Specify `nil` if you don’t want the document attributes.

## Return Value

Returns an initialized attributed string object, or `nil` if the method can’t decode the data.

## See Also

### Creating from RTF

init?(RTF: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string by decoding the stream of RTF commands and data in the specified data object.

init?(RTFDFileWrapper: FileWrapper, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from the specified file wrapper that contains an RTFD document.

