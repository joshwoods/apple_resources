

- UIKit
- UIPrintError
-  noContent 

Type Property

# noContent

UIKit hasn’t assigned a print formatter, page renderer, or printing item to print.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
static var noContent: UIPrintError.Code { get }
```

## See Also

### Accessing error codes

enum Code

Constants that specify the print error code.

static var notAvailable: UIPrintError.Code

The device doesn’t support printing.

static var unknownImageFormat: UIPrintError.Code

An image is in a format that UIKit doesn’t recognize for printing.

static var jobFailed: UIPrintError.Code

An internal error occurred with the print job.

