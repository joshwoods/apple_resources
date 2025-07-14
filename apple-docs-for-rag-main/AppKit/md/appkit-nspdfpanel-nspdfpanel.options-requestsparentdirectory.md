

- AppKit
- NSPDFPanel
- NSPDFPanel.Options
-  requestsParentDirectory 

Type Property

# requestsParentDirectory

The PDF panel doesn’t show a name field; instead, it allows the user to identify a directory in which to save multiple PDF files. If you set this flag, you’re responsible for appending a filename and the “pdf” extension to the resulting URL value in the NSPDFInfo object before proceeding with the creation of the PDF file (or calling the `takeSettingsFromPDFInfo` method of NSPrintInfo).

macOS 10.9+

``` source
static var requestsParentDirectory: NSPDFPanel.Options { get }
```

## See Also

### Constants

static var showsPaperSize: NSPDFPanel.Options

The PDF panel shows a menu of paper sizes.

static var showsOrientation: NSPDFPanel.Options

The PDF panel shows the current orientation of the PDF contents, such as landscape or portrait.

