

- UIKit
- UIDocumentBrowserError
-  UIDocumentBrowserError.Code 

Enumeration

# UIDocumentBrowserError.Code

The error codes for document browser errors.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error codes

case generic

An unspecified error.

case noLocationAvailable

An error indicating that no location exists.

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

### Related Documentation

class UIDocumentBrowserViewController

A view controller for browsing and performing actions on documents that you store locally and in the cloud.

### Handling errors

struct UIDocumentBrowserError

A structure that contains information about document browser errors.

let UIDocumentBrowserErrorDomain: String

The error domain for document browser errors.

