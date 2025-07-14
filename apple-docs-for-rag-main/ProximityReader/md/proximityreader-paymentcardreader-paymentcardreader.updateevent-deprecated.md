

- ProximityReader
- PaymentCardReader
-  PaymentCardReader.UpdateEvent Deprecated

Enumeration

# PaymentCardReader.UpdateEvent

An event you receive during the configuration of the payment system.

iOS 15.4–16.0DeprecatediPadOS 15.4–16.0DeprecatedMac Catalyst 17.0–17.0Deprecated

``` source
enum UpdateEvent
```

Deprecated

Use PaymentCardReader.Event

## Overview

If the prepare(using:updateHandler:) must update the device’s configuration, it delivers events to the update handler you provided. Use those events to monitor the status of the update.

## Topics

### Enumeration Cases

case notReady

A reader that is not ready to perform transactions.

case progress(Int)

The current update progress, specified as an integer value from 1 to 100.

### Instance Properties

var name: String

The name of the event.

## Relationships

### Conforms To

- Sendable

## See Also

### Deprecated

let id: String

A unique identifier for this object.

Deprecated

func prepare(using: PaymentCardReader.Token, updateHandler: ((PaymentCardReader.UpdateEvent) -> Void)?) async throws -> PaymentCardReaderSession

Configures the pipeline for reading payment or loyalty cards.

Deprecated

