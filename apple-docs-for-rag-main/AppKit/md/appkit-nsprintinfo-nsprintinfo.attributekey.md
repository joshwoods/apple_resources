

- AppKit
- NSPrintInfo
-  NSPrintInfo.AttributeKey 

Structure

# NSPrintInfo.AttributeKey

Constants that specify print job attributes.

macOS

``` source
struct AttributeKey
```

## Topics

### Page Setup Attributes

static let paperName: NSPrintInfo.AttributeKey

An `NSString` object containing the paper name.

static let paperSize: NSPrintInfo.AttributeKey

An `NSSize` value specifying the height and width of paper in points.

static let orientation: NSPrintInfo.AttributeKey

An `NSNumber` object containing an `NSPrintingOrientation`.

static let scalingFactor: NSPrintInfo.AttributeKey

Scale factor percentage before pagination.

### Pagination Attributes

static let leftMargin: NSPrintInfo.AttributeKey

`NSNumber`, containing a floating-point value that specifies the left margin, in points.

static let rightMargin: NSPrintInfo.AttributeKey

`NSNumber`, containing a floating-point value that specifies the right margin, in points.

static let topMargin: NSPrintInfo.AttributeKey

`NSNumber`, containing a floating-point value that specifies the top margin, in points.

static let bottomMargin: NSPrintInfo.AttributeKey

`NSNumber`, containing a floating-point value that specifies the bottom margin, in points.

static let horizontallyCentered: NSPrintInfo.AttributeKey

`NSNumber`, containing a Boolean value that is true if pages are centered horizontally.

static let verticallyCentered: NSPrintInfo.AttributeKey

`NSNumber`, containing a Boolean value that is true if pages are centered vertically.

static let horizontalPagination: NSPrintInfo.AttributeKey

`NSNumber`, containing a `NSPrintingPaginationMode` value.

static let verticalPagination: NSPrintInfo.AttributeKey

`NSNumber`, containing a `NSPrintingPaginationMode` value.

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

static let jobDisposition: NSPrintInfo.AttributeKey

An `NSString` object that specifies the job disposition.

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

static let selectionOnly: NSPrintInfo.AttributeKey

An `NSNumber` object containing a Boolean value—if true only the current selection is printed.

static let time: NSPrintInfo.AttributeKey

An `NSDate` object that specifies the time at which printing should begin.

### Initializers

init(String)

Creates a print job attribute key.

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

