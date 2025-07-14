

- AppKit
- NSPrintInfo
- NSPrintInfo.AttributeKey
-  jobDisposition 

Type Property

# jobDisposition

An `NSString` object that specifies the job disposition.

macOS

``` source
static let jobDisposition: NSPrintInfo.AttributeKey
```

## Discussion

`NSPrintSpoolJob`, `NSPrintPreviewJob`, `NSPrintSaveJob`, or `NSPrintCancelJob`. See jobDisposition for details.

## See Also

### Other Attributes

static let allPages: NSPrintInfo.AttributeKey

An `NSNumber` object containing a Boolean value—if true, includes all pages in output.

static let copies: NSPrintInfo.AttributeKey

An `NSNumber` object containing an integer—the number of copies to spool.

static let detailedErrorReporting: NSPrintInfo.AttributeKey

An `NSNumber` object containing a Boolean value—if true, produce detailed reports when an error occurs.

static let faxNumber: NSPrintInfo.AttributeKey

An `NSString` object that specifies a fax number.

static let firstPage: NSPrintInfo.AttributeKey

An `NSNumber` object containing an integer value that specifies the first page in the print job.

static let headerAndFooter: NSPrintInfo.AttributeKey

An `NSNumber` object containing a Boolean value—if true, a standard header and footer are added outside the margins of each page.

static let jobSavingFileNameExtensionHidden: NSPrintInfo.AttributeKey

A Boolean NSNumber indicating whether the job’s file name extension should be hidden when the jobDisposition is save. The default is false.

static let jobSavingURL: NSPrintInfo.AttributeKey

An `NSURL` containing the location to which the job file will be saved when the jobDisposition is save.

static let lastPage: NSPrintInfo.AttributeKey

An `NSNumber` object containing an integer value that specifies the last page in the print job.

static let mustCollate: NSPrintInfo.AttributeKey

An `NSNumber` object containing a Boolean value—if true, collates output.

static let pagesAcross: NSPrintInfo.AttributeKey

An `NSNumber` object that specifies the number of logical pages to be tiled horizontally on a physical sheet of paper.

static let pagesDown: NSPrintInfo.AttributeKey

An `NSNumber` object that specifies the number of logical pages to be tiled vertically on a physical sheet of paper.

static let printer: NSPrintInfo.AttributeKey

An `NSPrinter` object—the printer to use.

static let printerName: NSPrintInfo.AttributeKey

An `NSString` object that specifies the name of a printer.

static let reversePageOrder: NSPrintInfo.AttributeKey

An `NSNumber` object containing a Boolean value—if true, prints first page last.

