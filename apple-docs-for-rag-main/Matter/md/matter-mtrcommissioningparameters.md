

- Matter
-  MTRCommissioningParameters 

Class

# MTRCommissioningParameters

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRCommissioningParameters
```

## Topics

### Instance Properties

var attestationNonce: Data?

var countryCode: String?

var csrNonce: Data?Deprecated

var deviceAttestationDelegate: (any MTRDeviceAttestationDelegate)?

var failSafeExpiryTimeoutSecs: NSNumber?Deprecated

var failSafeTimeout: NSNumber?

var skipCommissioningComplete: Bool

var threadOperationalDataset: Data?

var wifiCredentials: Data?

var wifiSSID: Data?

var csrNonce: Data?

var readEndpointInformation: Bool

Read device type information from all endpoints during commissioning. Defaults to NO.

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

