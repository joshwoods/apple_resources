

- ProximityReader
-  StoreAndForwardPaymentCardReaderSession 

Class

# StoreAndForwardPaymentCardReaderSession

The object you use to start reading a contactless payment or loyalty card in Store and Forward mode.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
class StoreAndForwardPaymentCardReaderSession
```

## Overview

Use a `StoreAndForwardPaymentCardReaderSession` object to read payment and loyalty cards from a properly configured device. You don’t create this object directly. Instead, you obtain one by calling the prepareStoreAndForward() method of your PaymentCardReader object, which returns a session after the successful configuration of the device.

Maintain a strong reference to a session object for the duration of the card-reading process. You may use the same session object to perform multiple read operations, but you may perform only one read operation at a time

## Topics

### Instance Methods

func decline() async throws

Removes the last read from store.

func status() async throws -> StoreAndForwardStatus

Allows the merchant to check the status of the Store and Forward session.

## Relationships

### Inherits From

- PaymentCardReaderSession

### Conforms To

- Sendable

