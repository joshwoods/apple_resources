

- PassKit (Apple Pay and Wallet)
-  PKVehicleConnectionDelegate 

Protocol

# PKVehicleConnectionDelegate

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOSvisionOS 1.0+watchOS 8.5+

``` source
protocol PKVehicleConnectionDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func sessionDidChange(PKVehicleConnectionSessionConnectionState)

**Required**

func sessionDidReceive(Data)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Digital car keys

class PKAddCarKeyPassConfiguration

A specialized configuration object that PassKit uses when it creates a digital car key.

class PKVehicleConnectionSession

enum PKVehicleConnectionSessionConnectionState

