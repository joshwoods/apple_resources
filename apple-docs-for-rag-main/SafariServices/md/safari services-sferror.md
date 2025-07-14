

- Safari Services
-  SFError 

Structure

# SFError

A content blocker or Safari app extension error.

iOS 10.0+iPadOS 10.0+visionOS 1.0+

``` source
struct SFError
```

## Topics

### Error Codes

static var loadingInterrupted: SFError.Code

static var noAttachmentFound: SFError.Code

static var noExtensionFound: SFError.Code

enum Code

Messages that describe a content blocker or Safari app extension error.

### Error Domain

let SFErrorDomain: String

The domain for content blocker or Safari app extension errors.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Miscellaneous errors

enum Code

Messages that describe a content blocker or Safari app extension error.

let SFErrorDomain: String

The domain for content blocker or Safari app extension errors.

