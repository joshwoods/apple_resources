

- MailKit
- MEComposeSessionError
-  invalidBody 

Type Property

# invalidBody

An error that indicates the message’s body is invalid.

macOS 12.0+

``` source
static var invalidBody: MEComposeSessionError.Code { get }
```

## See Also

### Indicating Erroneous States

static var invalidHeaders: MEComposeSessionError.Code

An error that indicates one or more of the message’s headers are invalid.

static var invalidRecipients: MEComposeSessionError.Code

An error that indicates one or more of the message’s recipients are invalid.

let MEComposeSessionErrorDomain: String

A constant for the compose session error domain.

