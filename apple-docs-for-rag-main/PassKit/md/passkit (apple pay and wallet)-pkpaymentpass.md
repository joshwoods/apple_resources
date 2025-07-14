

- PassKit (Apple Pay and Wallet)
-  PKPaymentPass 

Class

# PKPaymentPass

An object that represents a provisioned payment card for in-app payments.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
class PKPaymentPass
```

## Overview

Use PKSecureElementPass in apps instead of this class to implement a payment pass in apps with these these system versions:

- iOS 13.4 or later

- macOS 11.0 or later

- watchOS 6.2 or later

- Mac Catalyst 13.4 or later

## Topics

### Determining activation state

var activationState: PKPaymentPassActivationState

The current activation state of the pass.

Deprecated

enum PKPaymentPassActivationState

Cases that indicate payment pass activation states.

Deprecated

## Relationships

### Inherits From

- PKSecureElementPass

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Payment passes

class PKAddPaymentPassViewController

Displays an interface that lets users add cards to Apple Pay from within your app.

