

- UIKit
- UIPrinter
-  UIPrinter.JobTypes 

Structure

# UIPrinter.JobTypes

Constants that indicate the types of jobs that the printer supports.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct JobTypes
```

## Topics

### Constants

static var unknown: UIPrinter.JobTypes

The printer support is unknown.

static var document: UIPrinter.JobTypes

The printer supports standard document printing.

static var envelope: UIPrinter.JobTypes

The printer supports printing on envelopes.

static var label: UIPrinter.JobTypes

The printer supports printing on cut labels.

static var photo: UIPrinter.JobTypes

The printer supports printing with photographic print quality.

static var receipt: UIPrinter.JobTypes

The printer supports printing receipts on a continuous roll of paper.

static var roll: UIPrinter.JobTypes

The printer supports printing documents or photos on a continuous roll of paper.

static var largeFormat: UIPrinter.JobTypes

The printer supports printing larger than the ISO A3 size.

static var postcard: UIPrinter.JobTypes

The printer supports printing on postcards.

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

## See Also

### Getting the printer information

var displayName: String

The human-readable printer name.

var displayLocation: String?

The human-readable text that describes the location of the printer.

var makeAndModel: String?

A string that contains the manufacturer’s name and the model name of the printer.

var supportedJobTypes: UIPrinter.JobTypes

The capabilities of the printer.

var supportsColor: Bool

A Boolean value that indicates whether the printer supports color printing.

var supportsDuplex: Bool

A Boolean value that indicates whether the printer supports printing on both sides of a sheet of paper.

