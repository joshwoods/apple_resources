

- UIKit
-  UIDocumentBrowserError 

Structure

# UIDocumentBrowserError

A structure that contains information about document browser errors.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct UIDocumentBrowserError
```

## Topics

### Error codes

static var generic: UIDocumentBrowserError.Code

An unspecified error.

static var noLocationAvailable: UIDocumentBrowserError.Code

An error indicating that no location exists.

enum Code

The error codes for document browser errors.

### Getting error properties

static var errorDomain: String

A string that identifies the error domain.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Handling errors

enum Code

The error codes for document browser errors.

let UIDocumentBrowserErrorDomain: String

The error domain for document browser errors.

