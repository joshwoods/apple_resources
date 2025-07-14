

- ManagedSettingsUI
-  ShieldConfigurationDataSource 

Class

# ShieldConfigurationDataSource

The base class for the principal object of an app extension that configures a shield’s appearance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@objc
class ShieldConfigurationDataSource
```

## Overview

You can create an extension to customize the appearance of the shields that the system uses to cover an application or website. The system provides your extension with the display names, bundle identifiers, and domains for each application, website, or category it shields. Your extension is expected to return an appropriate configuration as quickly as possible, in order to provide the best possible user experience. To protect the Family Sharing group’s privacy, your extension runs in a sandbox. This sandbox prevents your extension from making network requests or moving sensitive content outside the extension’s address space. The system provides a default appearance for any methods that your subclass doesn’t override, or if it takes too long to return a configuration.

## Topics

### Styling an Application Shield

func configuration(shielding: Application) -> ShieldConfiguration

Requests a configuration to use for a shield that covers an application.

func configuration(shielding: Application, in: ActivityCategory) -> ShieldConfiguration

Requests a configuration to use for a shield that covers an application because of its category.

### Styling a Website Shield

func configuration(shielding: WebDomain) -> ShieldConfiguration

Requests a configuration to use for a shield that covers a website.

func configuration(shielding: WebDomain, in: ActivityCategory) -> ShieldConfiguration

Requests a configuration to use for a shield that covers a website because of its category.

### Initializers

init()

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

## See Also

### Shield Configuration

struct ShieldConfiguration

An object that defines the appearance of a shield to display over an application or website.

