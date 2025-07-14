

- PassKit (Apple Pay and Wallet)
-  PKPass 

Class

# PKPass

An object that represents a single pass.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class PKPass
```

## Overview

The properties of this class correspond to fields of the pass. For details about what individual fields mean, see Pass.

## Topics

### Creating a pass

init(data: Data) throws

Creates a pass using the data you provide.

### Identifying a pass

var passType: PKPassType

The pass’s type.

enum PKPassType

Types of passes.

var secureElementPass: PKSecureElementPass?

The pass that contains an accompanying credential that the device stores in the Secure Element.

var serialNumber: String

A value that uniquely identifies the pass.

var passTypeIdentifier: String

The pass’s pass type identifier.

var deviceName: String

The name of the device that hosts the pass.

var localizedName: String

The localized name for the pass’s template.

var localizedDescription: String

The pass’s localized description.

var isRemotePass: Bool

A Boolean value that indicates whether the pass is on a paired device, such as an Apple Watch.

var paymentPass: PKPaymentPass?

The underlying payment pass.

Deprecated

### Getting the web service information

var webServiceURL: URL?

The URL for the web service.

var authenticationToken: String?

The token for authenticating update requests.

### Getting the display attributes

var icon: UIImage

The pass icon.

func localizedValue(forFieldKey: String) -> Any?

Returns the localized value for a specified field of the pass.

var organizationName: String

The name of the organization that creates the pass.

var relevantDate: Date?

The date when the pass is most likely to be useful or necessary.

Deprecated

### Getting the Wallet URL

var passURL: URL?

The URL that opens the pass in the Wallet app.

### Providing contextual information

var userInfo: [AnyHashable : Any]?

Developer-specific custom data.

### Instance Properties

var relevantDates: [PKPassRelevantDate]

## Relationships

### Inherits From

- PKObject

### Inherited By

- PKSecureElementPass

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### General purpose passes

class PKSecureElementPass

A pass with a credential that the device stores in a certified payment information chip.

class PKAddSecureElementPassConfiguration

An object that describes the configuration of a secure element payment pass.

class PKAddSecureElementPassViewController

A view controller that manages the addition of secure element payment passes.

class PKAddPassesViewController

Lets your app show a pass and prompt the user to add that pass to the pass library.

struct AsyncShareablePassConfiguration

class PKShareSecureElementPassViewController

protocol PKShareSecureElementPassViewControllerDelegate

class Preview

enum PKShareSecureElementPassResult

