

- Safari Services
-  SFError.Code 

Enumeration

# SFError.Code

Messages that describe a content blocker or Safari app extension error.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.4+macOS 10.12+visionOS 1.0+

**iOS, iPadOS, visionOS**

``` source
enum Code
```

**Mac Catalyst, macOS**

``` source
enum SFErrorCode
```

## Topics

### Error Codes

case loadingInterrupted

There was an error loading the content blocker extension.

case noAttachmentFound

The Content Blocker extension returned an NSExtensionItem that did not include an attachment.

case noExtensionFound

A Content Blocker or Safari app extension with the specified bundle identifier was not found, or the bundle identifier specified an extension that was not owned by you.

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

### Miscellaneous errors

struct SFError

A content blocker or Safari app extension error.

let SFErrorDomain: String

The domain for content blocker or Safari app extension errors.

