

- Message UI
- MFMailComposeError
-  MFMailComposeError.Code 

Enumeration

# MFMailComposeError.Code

Error codes for NSError objects that are associated with the mail composition interface.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Code
```

## Topics

### Constants

case saveFailed

An error occurred while trying to save the email message to the Drafts folder.

case sendFailed

An error occurred while trying to queue or send the email message.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Responding to errors

struct MFMailComposeError

Mail composition errors.

let MFMailComposeErrorDomain: String

The domain used for error objects that are associated with the mail composition interface.

