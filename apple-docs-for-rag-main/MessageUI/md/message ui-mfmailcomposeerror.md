

- Message UI
-  MFMailComposeError 

Structure

# MFMailComposeError

Mail composition errors.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct MFMailComposeError
```

## Topics

### Errors

static var errorDomain: String

The domain for errors related to mail composition.

static var saveFailed: MFMailComposeError.Code

An error occurred while trying to save the email message to the drafts folder.

static var sendFailed: MFMailComposeError.Code

An error occurred while trying to queue or send the email message.

enum Code

Error codes for NSError objects that are associated with the mail composition interface.

### Error Configuration

static var errorDomain: String

The domain for errors related to mail composition.

var localizedDescription: String

Retrieve the localized description for this error.

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Responding to errors

let MFMailComposeErrorDomain: String

The domain used for error objects that are associated with the mail composition interface.

enum Code

Error codes for NSError objects that are associated with the mail composition interface.

