

- PassKit (Apple Pay and Wallet)
-  PKVehicleConnectionSession 

Class

# PKVehicleConnectionSession

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOSvisionOS 1.0+watchOS 8.5+

``` source
class PKVehicleConnectionSession
```

## Topics

### Instance Properties

var connectionStatus: PKVehicleConnectionSessionConnectionState

var delegate: (any PKVehicleConnectionDelegate)?

### Instance Methods

func invalidate()

func send(Data) throws

### Type Methods

class func session(for: PKSecureElementPass, delegate: any PKVehicleConnectionDelegate, completion: (PKVehicleConnectionSession?, (any Error)?) -> Void)

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

### Digital car keys

class PKAddCarKeyPassConfiguration

A specialized configuration object that PassKit uses when it creates a digital car key.

protocol PKVehicleConnectionDelegate

enum PKVehicleConnectionSessionConnectionState

