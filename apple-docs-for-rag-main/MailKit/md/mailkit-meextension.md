

- MailKit
-  MEExtension 

Protocol

# MEExtension

A type that provides objects for manipulating email messages, such as performing actions on messages or blocking content when users view messages.

macOS 12.0+

``` source
@MainActor
protocol MEExtension : NSObjectProtocol
```

## Overview

To implement an app extension, you provide an object that conforms to the MEExtension protocol. The MEExtensionCapabilities key of your extension’s `Info.plist` defines the capabilities that you support, as follows:

```
NSExtensionAttributes

    MEExtensionCapabilities

        MEContentBlocker
        MEMessageActionHandler
        MEComposeSessionHandler
        MEMessageSecurityHandler

```

For each capability that your extension defines, you provide an object that implements the capability. MailKit uses the following methods to request the object for a given capability. The capability also specifies a protocol that the handler implements.

| Capability Key | Method | Protocol |
|----|----|----|
| `MEContentBlocker` | handler(for:) | MEContentBlocker |
| `MEMessageActionHandler` | handlerForMessageActions() | MEMessageActionHandler |
| `MEComposeSessionHandler` | handlerForContentBlocker() | MEComposeSessionHandler |
| `MEMessageSecurityHandler` | handlerForMessageSecurity() | MEMessageSecurityHandler |

## Topics

### Blocking Content

func handlerForContentBlocker() -> any MEContentBlocker

Returns an object that provides rules that the message viewer uses to block content.

### Performing Actions on Messages

func handlerForMessageActions() -> any MEMessageActionHandler

Returns an object that performs actions on mail messages as the system downloads them.

### Enhancing the Compose Window

func handler(for: MEComposeSession) -> any MEComposeSessionHandler

Returns an object that participates in the composition of a mail message.

### Encrypting and Signing Messages

func handlerForMessageSecurity() -> any MEMessageSecurityHandler

Returns an object that applies security measures such as encryption and digital signatures to messages.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Essentials

Build Mail App Extensions

Create app extensions that block content, perform message and composing actions, and help message security.

