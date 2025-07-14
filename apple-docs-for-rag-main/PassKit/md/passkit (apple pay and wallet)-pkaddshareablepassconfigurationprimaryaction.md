

- PassKit (Apple Pay and Wallet)
-  PKAddShareablePassConfigurationPrimaryAction 

Enumeration

# PKAddShareablePassConfigurationPrimaryAction

The kind of add action that the system performs with a pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
enum PKAddShareablePassConfigurationPrimaryAction
```

## Topics

### Shareable pass configuration actions

case add

A constant that indicates the system adds a pass to a device.

case share

A constant that indicates the system shares the pass with another user.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Shareable passes

class PKAddShareablePassConfiguration

An object that represents the data and action for a shared copy of pass.

class PKShareablePassMetadata

Information that you use to configure the sharing sheet for a pass.

