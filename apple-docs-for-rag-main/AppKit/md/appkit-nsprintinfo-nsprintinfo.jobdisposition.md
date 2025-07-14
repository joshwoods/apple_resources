

- AppKit
- NSPrintInfo
-  NSPrintInfo.JobDisposition 

Structure

# NSPrintInfo.JobDisposition

Constants that specify values for the print job disposition.

macOS

``` source
struct JobDisposition
```

## Discussion

These constants are used by the jobDisposition property.

## Topics

### Constants

static let spool: NSPrintInfo.JobDisposition

Normal print job.

static let preview: NSPrintInfo.JobDisposition

Send to Preview application.

static let save: NSPrintInfo.JobDisposition

Save to a file.

static let cancel: NSPrintInfo.JobDisposition

Cancel print job.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Controlling Printing

var jobDisposition: NSPrintInfo.JobDisposition

The action specified for the job.

func setUpPrintOperationDefaultValues()

Validates the attributes encapsulated by the print info.

