

- Core Graphics
- CGPSConverterCallbacks
-  endPage 

Instance Property

# endPage

The callback called at the end of the conversion of each page in the PostScript document, or `NULL`.

Mac CatalystmacOS

``` source
var endPage: CGPSConverterEndPageCallback?
```

## See Also

### Instance Properties

var beginDocument: CGPSConverterBeginDocumentCallback?

The callback called at the beginning of the conversion of the PostScript document, or `NULL`.

var beginPage: CGPSConverterBeginPageCallback?

The callback called at the start of the conversion of each page in the PostScript document, or `NULL`.

var endDocument: CGPSConverterEndDocumentCallback?

The callback called at the end of conversion of the PostScript document, or `NULL`.

var noteMessage: CGPSConverterMessageCallback?

The callback called to pass any messages that might result during the conversion, or `NULL`.

var noteProgress: CGPSConverterProgressCallback?

The callback called periodically during the conversion to indicate that conversion is proceeding, or `NULL`.

var releaseInfo: CGPSConverterReleaseInfoCallback?

The callback called when the converter is deallocated, or `NULL`.

var version: UInt32

The version number of the structure passed in as a parameter to the converter creation functions. The structure defined below is version `0`.

