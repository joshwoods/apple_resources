

- PassKit (Apple Pay and Wallet)
-  PKAddShareablePassConfiguration 

Class

# PKAddShareablePassConfiguration

An object that represents the data and action for a shared copy of pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
class PKAddShareablePassConfiguration
```

## Topics

### Creating a pass configuration

class func forPassMetaData([PKShareablePassMetadata], provisioningPolicyIdentifier: String, action: PKAddShareablePassConfigurationPrimaryAction, completion: (PKAddShareablePassConfiguration?, (any Error)?) -> Void)

Creates and error checks a new shareable pass-configuration object.

Deprecated

var primaryAction: PKAddShareablePassConfigurationPrimaryAction

The action that the system performs with the shareable pass.

var credentialsMetadata: [PKShareablePassMetadata]

Information for a shareable pass.

var provisioningPolicyIdentifier: StringDeprecated

### Type Methods

class func forPassMetadata([PKShareablePassMetadata], action: PKAddShareablePassConfigurationPrimaryAction, completion: (PKAddShareablePassConfiguration?, (any Error)?) -> Void)

## Relationships

### Inherits From

- PKAddSecureElementPassConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Shareable passes

class PKShareablePassMetadata

Information that you use to configure the sharing sheet for a pass.

enum PKAddShareablePassConfigurationPrimaryAction

The kind of add action that the system performs with a pass.

