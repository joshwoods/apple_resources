

- MailKit
-  MEComposeSessionHandler 

Protocol

# MEComposeSessionHandler

An object that participates in the composition of mail messages, and annotates recipient tokens.

macOS 12.0+

``` source
@MainActor
protocol MEComposeSessionHandler : NSObjectProtocol
```

## Overview

When the user composes a message, MailKit requests a compose session handler object from your extension. MailKit uses this handler in the following ways:

- To inform it when the compose session begins and ends

- To add status annotations for email addresses that the user enters into the To, Cc, and Bcc fields

- To display a custom popover in the compose window

- To include custom headers in an outgoing message

- To confirm that an outgoing message is ready for delivery

Each of the items in the list above corresponds to methods that the handler implements.

To indicate that your extension contains a compose session handler, add `MEComposeSessionHandler` to the MEExtensionCapabilities array in the extension’s `Info.plist` file:

```
```

## Topics

### Handling Compose Sessions

class MEComposeSession

An object that represents a single mail compose window.

func mailComposeSessionDidBegin(MEComposeSession)

Informs the handler when the user opens a compose window.

**Required**

func mailComposeSessionDidEnd(MEComposeSession)

Informs the handler when the user closes a compose window.

**Required**

struct MEComposeSessionError

An error that indicates the compose session is in an erroneous state.

### Annotating Email Address Tokens

func annotateAddressesForSession(MEComposeSession, completion: ([MEEmailAddress : MEAddressAnnotation]) -> Void)

Indicates whether recipients in the compose window are valid or not.

class MEAddressAnnotation

An object that indicates the validity of an email address.

### Extending the Compose Window Interface

func viewController(for: MEComposeSession) -> MEExtensionViewController

Provides a custom view controller to display as part of the compose window.

**Required**

### Adding Custom Headers

func additionalHeaders(for: MEComposeSession) -> [String : [String]]

Provides custom headers to include in the outgoing message.

### Approving Message Delivery

func allowMessageSendForSession(MEComposeSession, completion: ((any Error)?) -> Void)

Confirms that the message is ready for delivery.

## Relationships

### Inherits From

- NSObjectProtocol

