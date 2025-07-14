

- AppKit
- NSPDFInfo
-  attributes 

Instance Property

# attributes

A dictionary of additional attributes that describe how to export content as a PDF file.

macOS 10.9+

``` source
var attributes: NSMutableDictionary { get }
```

## Discussion

Although `attributes` is a read-only property, you can modify the mutable dictionary associated with it. Typically, this dictionary contains custom attributes or parameters that are set by a custom accessory view in the PDF panel.

## See Also

### Specifying PDF Information

var url: URL?

The URL identifying the location at which the PDF file will be created.

var isFileExtensionHidden: Bool

A Boolean value that indicates whether the file extension should appear after the filename.

var tagNames: [String]

An array of tag names that should be applied to the PDF file after it’s created.

var orientation: NSPrintInfo.PaperOrientation

The paper orientation to use when exporting content as a PDF file.

var paperSize: NSSize

The paper size to use when exporting content as a PDF file.

