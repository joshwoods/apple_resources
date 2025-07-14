

- AppKit
-  NSPrintInfo 

Class

# NSPrintInfo

An object that stores information that’s used to generate printed output.

macOS

``` source
class NSPrintInfo
```

## Overview

A shared NSPrintInfo object is automatically created for an app and is used by default for all printing jobs for that app. The printing information in an NSPrintInfo object is stored in a dictionary. To access the standard attributes in the dictionary directly, this class defines a set of keys and provides the dictionary() method. You can also initialize an instance of this class using the init(dictionary:) method.

You can use this dictionary to store custom information associated with a print job. Any non-object values should be stored as NSNumber or NSValue objects in the dictionary. See NSNumber for a list of types which should be stored as numbers. For other non-object values, use the NSValue class.

To store custom information that belongs in printing presets you should use the dictionary returned by the printSettings method.

## Topics

### Creating the Printing Information Object

class var shared: NSPrintInfo

The shared printing information object.

init(dictionary: [NSPrintInfo.AttributeKey : Any])

Returns a printing information object initialized with the parameters in the specified dictionary.

convenience init()

Creates a printing information object.

init(coder: NSCoder)

Creates a printing information object from data in an unarchiver.

### Managing the Printing Rectangle

var paperSize: NSSize

The size of the paper.

var topMargin: CGFloat

The top margin to the specified size.

var bottomMargin: CGFloat

The height of the bottom margin.

var leftMargin: CGFloat

The width of the left margin.

var rightMargin: CGFloat

The width of the right margin.

var imageablePageBounds: NSRect

The imageable area of a sheet of paper specified by the print info.

var orientation: NSPrintInfo.PaperOrientation

The orientation attribute.

enum PaperOrientation

Constants that describe the orientation of printing on a page.

var paperName: NSPrinter.PaperName?

The name of the currently selected paper size.

struct PaperName

The type you use to specify the name of a type of paper.

var localizedPaperName: String?

The human-readable name of the currently selected paper size, suitable for presentation in user interfaces.

### Pagination

var horizontalPagination: NSPrintInfo.PaginationMode

The horizontal pagination mode.

var verticalPagination: NSPrintInfo.PaginationMode

The vertical pagination to the specified mode.

enum PaginationMode

Constants that specify the different ways in which an image is divided into pages.

### Positioning the Image on the Page

var isHorizontallyCentered: Bool

A Boolean value that indicates whether the image is centered horizontally.

var isVerticallyCentered: Bool

A Boolean value that indicates whether the image is centered vertically.

### Specifying the Printer

var printer: NSPrinter

The printer object to be used for printing.

class NSPrinter

An object that describes a printer’s capabilities.

### Controlling Printing

var jobDisposition: NSPrintInfo.JobDisposition

The action specified for the job.

struct JobDisposition

Constants that specify values for the print job disposition.

func setUpPrintOperationDefaultValues()

Validates the attributes encapsulated by the print info.

### Accessing the Print Info Dictionary

func dictionary() -> NSMutableDictionary

Returns the print info’s dictionary that contains the printing attributes.

### Print Settings Convenience Methods

var isSelectionOnly: Bool

A Boolean value that indicates whether only the currently selected contents should be printed.

var scalingFactor: CGFloat

The current scaling factor.

### Accessing Core Printing Information

var printSettings: NSMutableDictionary

A mutable dictionary containing the print settings from Core Printing.

typealias SettingKey

The type you use to specify a print info setting key.

func pmPrintSession() -> UnsafeMutableRawPointer

Returns a Core Printing object configured with the print info’s session information.

func pmPageFormat() -> UnsafeMutableRawPointer

Returns a Core Printing object configured with the print info’s page format information.

func pmPrintSettings() -> UnsafeMutableRawPointer

Returns a Core Printing object configured with the print info’s print settings information

func updateFromPMPageFormat()

Synchronizes the print info’s page format information with information from its associated page format object.

func updateFromPMPrintSettings()

Synchronizes the print info’s print settings information with information from its associated print settings object.

func takeSettings(from: NSPDFInfo)

Updates the print info with all the settings and attributes in the specified PDF info object.

### Constants

struct AttributeKey

Constants that specify print job attributes.

### Deprecated

class var defaultPrinter: NSPrinter?

Deprecated.

enum Orientation

Constants that specify page orientations.

Deprecated

Deprecated Printing Keys

These keys refer to older printing properties that are no longer used.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Print Information

class NSPrinter

An object that describes a printer’s capabilities.

class NSPrintOperation

An object that controls operations that generate Encapsulated PostScript (EPS) code, Portable Document Format (PDF) code, or print jobs.

