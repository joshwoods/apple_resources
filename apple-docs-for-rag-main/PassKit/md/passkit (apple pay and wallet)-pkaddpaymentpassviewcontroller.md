

- PassKit (Apple Pay and Wallet)
-  PKAddPaymentPassViewController 

Class

# PKAddPaymentPassViewController

Displays an interface that lets users add cards to Apple Pay from within your app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class PKAddPaymentPassViewController
```

## Overview

Important

Adding payment passes requires a special entitlement issued by Apple. Your app must include this entitlement before this class can be instantiated. For more information on requesting this entitlement, see the Card Issuers section at developer.apple.com/apple-pay/.

## Topics

### Determining if payment passes can be added

class func canAddPaymentPass() -> Bool

Returns a Boolean value that indicates whether the app can add cards to Apple Pay.

### Working with add payment view controllers

var delegate: (any PKAddPaymentPassViewControllerDelegate)?

The object that acts as the delegate for the add payment view controller.

protocol PKAddPaymentPassViewControllerDelegate

Methods that let the system prompt you for an add payment request, and inform you when a request has succeeded or failed.

### Creating an add-payment-pass view controller

init?(requestConfiguration: PKAddPaymentPassRequestConfiguration, delegate: (any PKAddPaymentPassViewControllerDelegate)?)

Returns an initialized add payment view controller object, using the provided configuration and delegate.

class PKAddPaymentPassRequestConfiguration

Contains the configuration data for a view controller that lets the user add a payment pass.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Payment passes

class PKPaymentPass

An object that represents a provisioned payment card for in-app payments.

