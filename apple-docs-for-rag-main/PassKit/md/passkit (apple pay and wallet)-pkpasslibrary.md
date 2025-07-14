

- PassKit (Apple Pay and Wallet)
-  PKPassLibrary 

Class

# PKPassLibrary

Provides an interface to the user’s library of passes.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
class PKPassLibrary
```

## Overview

The `PKPassLibrary` isn’t thread-safe. Use instances of this class only on a single thread.

## Topics

### Accessing passes

class func isPassLibraryAvailable() -> Bool

Returns a Boolean value that indicates whether the pass library is available.

func passes() -> [PKPass]

Returns the passes in the user’s pass library that the app can access.

func passes(of: PKPassType) -> [PKPass]

Returns the passes of the specified pass type.

func pass(withPassTypeIdentifier: String, serialNumber: String) -> PKPass?

Returns the pass with the specified pass type identifier and serial number.

func containsPass(PKPass) -> Bool

Returns a Boolean value that indicates whether the user’s pass library contains the specified pass.

func serviceProviderData(for: PKSecureElementPass, completion: (Data?, (any Error)?) -> Void)

Calls a completion handler that returns the custom data for a Secure Element pass.

var remoteSecureElementPasses: [PKSecureElementPass]

The Secure Element passes that PassKit stores on paired devices.

### Adding passes

func canAddSecureElementPass(primaryAccountIdentifier: String) -> Bool

Returns a Boolean value that indicates whether PassKit can add a Secure Element pass for the specified account.

func canAddFelicaPass() -> Bool

Returns a Boolean value that indicates whether the library can add FeliCa™ passes.

func addPasses([PKPass], withCompletionHandler: ((PKPassLibraryAddPassesStatus) -> Void)?)

Presents a user interface for adding multiple passes at once.

enum PKPassLibraryAddPassesStatus

Statuses that PassKit uses when it adds passes to the pass library.

### Managing passes

var isSecureElementPassActivationAvailable: Bool

A Boolean value that indicates whether the device supports creating Secure Element passes.

func activate(PKSecureElementPass, activationData: Data, completion: ((Bool, (any Error)?) -> Void)?)

Activates a Secure Element pass using the specified data.

func replacePass(with: PKPass) -> Bool

Replaces a pass in the user’s pass library with the specified pass.

func removePass(PKPass)

Removes the pass from the user’s pass library.

### Presenting and suppressing passes

func present(PKSecureElementPass)

Presents a Secure Element pass.

class func isSuppressingAutomaticPassPresentation() -> Bool

Returns a Boolean value that indicates whether the system suppresses the automatic presentation of Apple Pay passes.

class func requestAutomaticPassPresentationSuppression(responseHandler: (PKAutomaticPassPresentationSuppressionResult) -> Void) -> PKSuppressionRequestToken

Prevents the device from automatically displaying the Apple Pay interface.

enum PKAutomaticPassPresentationSuppressionResult

The result of an attempt to suppress automatic pass presentation.

class func endAutomaticPassPresentationSuppression(withRequestToken: PKSuppressionRequestToken)

Reenables the automatic display of the Apple Pay interface.

typealias PKSuppressionRequestToken

A token that represents a request to suppress the automatic presentation of payment passes.

### Setting up payments

func openPaymentSetup()

Opens the user interface to set up credit cards for Apple Pay.

### Signing data

func sign(Data, using: PKSecureElementPass, completion: (Data?, Data?, (any Error)?) -> Void)

Signs an opaque value using a cryptographic signature.

### Receiving notifications

struct PKPassLibraryNotificationKey

The user info keys that a pass library notification uses.

struct PKPassLibraryNotificationName

The types of notifications that the pass library posts.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

### Instance Methods

func encryptedServiceProviderData(for: PKSecureElementPass, completion: ([AnyHashable : Any]?, (any Error)?) -> Void)

func passes(withReaderIdentifier: String) -> Set&lt;PKSecureElementPass>

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

