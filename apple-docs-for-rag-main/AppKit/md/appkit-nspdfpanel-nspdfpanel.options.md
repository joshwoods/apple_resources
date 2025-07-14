

- AppKit
- NSPDFPanel
-  NSPDFPanel.Options 

Structure

# NSPDFPanel.Options

Constants used to configure the contents of a PDF panel.

macOS 10.9+

``` source
struct Options
```

## Topics

### Constants

static var showsPaperSize: NSPDFPanel.Options

The PDF panel shows a menu of paper sizes.

static var showsOrientation: NSPDFPanel.Options

The PDF panel shows the current orientation of the PDF contents, such as landscape or portrait.

static var requestsParentDirectory: NSPDFPanel.Options

The PDF panel doesn’t show a name field; instead, it allows the user to identify a directory in which to save multiple PDF files. If you set this flag, you’re responsible for appending a filename and the “pdf” extension to the resulting URL value in the NSPDFInfo object before proceeding with the creation of the PDF file (or calling the `takeSettingsFromPDFInfo` method of NSPrintInfo).

### Initializers

init(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

