

- PassKit (Apple Pay and Wallet)
-  PKSecureElementPass 

Class

# PKSecureElementPass

A pass with a credential that the device stores in a certified payment information chip.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+watchOS 6.2+

``` source
class PKSecureElementPass
```

## Topics

### Getting the activation state

var passActivationState: PKSecureElementPass.PassActivationState

The activation state of the pass.

enum PassActivationState

The activation states of a Secure Element pass.

### Getting the hardware attributes

var deviceAccountIdentifier: String

The unique identifier for the device-specific account number.

var deviceAccountNumberSuffix: String

A display-ready version of the device-specific account number.

var devicePassIdentifier: String?

An opaque value for the pass.

var pairedTerminalIdentifier: String?

The unique identifier of the paired terminal.

### Getting the account attributes

var primaryAccountIdentifier: String

An opaque value that identifies the primary account number that funds the pass’s transactions.

var primaryAccountNumberSuffix: String

A display-ready version of the primary account number.

## Relationships

### Inherits From

- PKPass

### Inherited By

- PKPaymentPass

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### General purpose passes

class PKAddSecureElementPassConfiguration

An object that describes the configuration of a secure element payment pass.

class PKAddSecureElementPassViewController

A view controller that manages the addition of secure element payment passes.

class PKPass

An object that represents a single pass.

class PKAddPassesViewController

Lets your app show a pass and prompt the user to add that pass to the pass library.

struct AsyncShareablePassConfiguration

class PKShareSecureElementPassViewController

protocol PKShareSecureElementPassViewControllerDelegate

class Preview

enum PKShareSecureElementPassResult

