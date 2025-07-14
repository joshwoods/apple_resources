

- CryptoTokenKit
-  TKSmartCardTokenDriverDelegate 

Protocol

# TKSmartCardTokenDriverDelegate

The interface that a smart card token driver delegate implements to respond to token creation events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol TKSmartCardTokenDriverDelegate : TKTokenDriverDelegate
```

## Topics

### Delegate Methods

func tokenDriver(TKSmartCardTokenDriver, createTokenFor: TKSmartCard, aid: Data?) throws -> TKSmartCardToken

Tells the delegate that a new Smart Card is detected.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- TKTokenDriverDelegate

