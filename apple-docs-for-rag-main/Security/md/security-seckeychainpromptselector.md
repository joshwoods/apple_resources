

- Security
-  SecKeychainPromptSelector 

Structure

# SecKeychainPromptSelector

Bits that define when a keychain should require a passphrase.

macOS 10.0+

``` source
struct SecKeychainPromptSelector
```

## Topics

### Constants

static var requirePassphase: SecKeychainPromptSelector

Indicates that a passphrase should be required for every access.

static var unsigned: SecKeychainPromptSelector

Indicates that a passphrase should be required when an unsigned application attempts to use the keychain, overriding the system default.

static var unsignedAct: SecKeychainPromptSelector

Indicates that a passphrase should be required when an unsigned application attempts to use the keychain.

static var invalid: SecKeychainPromptSelector

Indicates that a passphrase should be required when an application with an invalid signature attempts to use the keychain, overriding the system default.

static var invalidAct: SecKeychainPromptSelector

Indicates that a passphrase should be required when an application with an invalid signature attempts to use the keychain.

### Initializers

init(rawValue: uint16)

Initializes a keychain prompt selector.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

