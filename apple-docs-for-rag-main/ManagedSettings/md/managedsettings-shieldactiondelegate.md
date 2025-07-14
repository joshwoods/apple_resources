

- ManagedSettings
-  ShieldActionDelegate 

Class

# ShieldActionDelegate

A class for an extension that handles shield actions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@objc
class ShieldActionDelegate
```

## Overview

Subclass `ShieldActionDelegate` to allow client extensions to respond to user actions on a shield that covers an application or website. The system doesn’t provide the name of a shielded Application, WebDomain, or ActivityCategory to preserve the Family Sharing group’s privacy. Instead, the system uses a token to indicate what content it is shielding.

## Topics

### Handling Shield Actions

enum ShieldAction

Constants that describe a user’s action for your extension to handle.

enum ShieldActionResponse

Constants your extension that handles shield actions can use to tell the system how to respond to an action.

### Initializers

init()

### Instance Methods

func handle(action: ShieldAction, for: ApplicationToken, completionHandler: (ShieldActionResponse) -> Void)

Allows the extension to respond to a user action when the system displays a shield over an application.

func handle(action: ShieldAction, for: WebDomainToken, completionHandler: (ShieldActionResponse) -> Void)

Allows the extension to respond to a user action when the system displays a shield over a website.

func handle(action: ShieldAction, for: ActivityCategoryToken, completionHandler: (ShieldActionResponse) -> Void)

Allows the extension to respond to a user action when the system displays a shield over an application or website because of its category.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

