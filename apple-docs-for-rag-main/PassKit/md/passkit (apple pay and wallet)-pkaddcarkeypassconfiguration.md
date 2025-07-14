

- PassKit (Apple Pay and Wallet)
-  PKAddCarKeyPassConfiguration 

Class

# PKAddCarKeyPassConfiguration

A specialized configuration object that PassKit uses when it creates a digital car key.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOSvisionOS 1.0+

``` source
class PKAddCarKeyPassConfiguration
```

## Topics

### Creating a pass configuration

init()

Creates a digital car key configuration object.

### Setting the wireless radio technology

var supportedRadioTechnologies: PKRadioTechnology

The wireless radio technology that the key uses.

struct PKRadioTechnology

Constants that describe the type of wireless radio technology that a pass uses.

### Managing the password

var password: String

A one-time password that the vehicle manufacturer provides.

### Setting the provisioning template

var provisioningTemplateIdentifier: String?

### Instance Properties

var manufacturerIdentifier: String

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

### Digital car keys

class PKVehicleConnectionSession

protocol PKVehicleConnectionDelegate

enum PKVehicleConnectionSessionConnectionState

