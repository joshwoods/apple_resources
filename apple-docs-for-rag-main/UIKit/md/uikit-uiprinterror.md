

- UIKit
-  UIPrintError 

Structure

# UIPrintError

A structure that contains information about a printing error.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct UIPrintError
```

## Topics

### Accessing error codes

enum Code

Constants that specify the print error code.

static var notAvailable: UIPrintError.Code

The device doesn’t support printing.

static var noContent: UIPrintError.Code

UIKit hasn’t assigned a print formatter, page renderer, or printing item to print.

static var unknownImageFormat: UIPrintError.Code

An image is in a format that UIKit doesn’t recognize for printing.

static var jobFailed: UIPrintError.Code

An internal error occurred with the print job.

### Getting error information

static var errorDomain: String

The printing error domain.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Handling printing errors

let UIPrintErrorDomain: String

The string constant that defines the UIKit printing error domain.

enum Code

Constants that specify the print error code.

