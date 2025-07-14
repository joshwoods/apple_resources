

- ProximityReader
- PaymentCardReader
-  prepare(using:updateHandler:) Deprecated

Instance Method

# prepare(using:updateHandler:)

Configures the pipeline for reading payment or loyalty cards.

iOS 15.4–16.0DeprecatediPadOS 15.4–16.0DeprecatedMac Catalyst 17.0–17.0Deprecated

``` source
func prepare(
    using token: PaymentCardReader.Token,
    updateHandler: ((PaymentCardReader.UpdateEvent) -> Void)?
) async throws -> PaymentCardReaderSession
```

Deprecated

Use events instead of passing in updateHandler

## Parameters 

`token`  

Valid and signed token from a participating payment service provider.

`updateHandler`  

Returns configuration progress or session state change.

## Return Value

PaymentCardReaderSession when successful.

## Discussion

Call this function to configure Tap to Pay on iPhone on someone’s device. This method verifies that the device is able to read contactless cards and is properly configured to process transactions.

Upon successful configuration of the device, this method returns a PaymentCardReaderSession object, which you use to read card information. The session remains active while your app is in the foreground. If you release the returned session, call this method again before you start any new read operations.

After calling this method, there are four possible scenarios:

- The method returns an existing PaymentCardReaderSession immediately if that session is still valid.

- The method retrieves and returns a new PaymentCardReaderSession from the server if the device is fully configured.

- The method updates the device’s configuration and delivers progress updates to the provided `updateHandler`. Upon completion, the method returns a new PaymentCardReaderSession for the updated configuration. This process can take anywhere from a few seconds to several minutes.

- This method throws a PaymentCardReaderError if a problem occurs.

Throws

PaymentCardReaderError if the method fails to configure the device.

## See Also

### Deprecated

let id: String

A unique identifier for this object.

Deprecated

enum UpdateEvent

An event you receive during the configuration of the payment system.

Deprecated

