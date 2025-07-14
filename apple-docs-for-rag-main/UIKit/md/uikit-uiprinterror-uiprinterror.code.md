

- UIKit
- UIPrintError
-  UIPrintError.Code 

Enumeration

# UIPrintError.Code

Constants that specify the print error code.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error codes

case notAvailable

The device doesn’t support printing.

case noContent

UIKit hasn’t assigned a print formatter, page renderer, or printing item to print.

case unknownImageFormat

An image is in a format that UIKit doesn’t recognize for printing.

case jobFailed

An internal error occurred with the print job.

### Global variables

Print error global variables

Global variables associated with print errors.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling printing errors

let UIPrintErrorDomain: String

The string constant that defines the UIKit printing error domain.

struct UIPrintError

A structure that contains information about a printing error.

