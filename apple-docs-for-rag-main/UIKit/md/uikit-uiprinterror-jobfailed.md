

- UIKit
- UIPrintError
-  jobFailed 

Type Property

# jobFailed

An internal error occurred with the print job.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
static var jobFailed: UIPrintError.Code { get }
```

## See Also

### Accessing error codes

enum Code

Constants that specify the print error code.

static var notAvailable: UIPrintError.Code

The device doesn’t support printing.

static var noContent: UIPrintError.Code

UIKit hasn’t assigned a print formatter, page renderer, or printing item to print.

static var unknownImageFormat: UIPrintError.Code

An image is in a format that UIKit doesn’t recognize for printing.

