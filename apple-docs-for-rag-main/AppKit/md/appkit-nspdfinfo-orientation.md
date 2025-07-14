

- AppKit
- NSPDFInfo
-  orientation 

Instance Property

# orientation

The paper orientation to use when exporting content as a PDF file.

macOS 10.9+

``` source
var orientation: NSPrintInfo.PaperOrientation { get set }
```

## See Also

### Specifying PDF Information

var url: URL?

The URL identifying the location at which the PDF file will be created.

var isFileExtensionHidden: Bool

A Boolean value that indicates whether the file extension should appear after the filename.

var tagNames: [String]

An array of tag names that should be applied to the PDF file after it’s created.

var paperSize: NSSize

The paper size to use when exporting content as a PDF file.

var attributes: NSMutableDictionary

A dictionary of additional attributes that describe how to export content as a PDF file.

