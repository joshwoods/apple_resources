

- ProximityReader
- PaymentCardReader
-  id Deprecated

Instance Property

# id

A unique identifier for this object.

iOS 15.4–16.0DeprecatediPadOS 15.4–16.0DeprecatedMac Catalyst 17.0–17.0Deprecated

``` source
final let id: String
```

Deprecated

Use ObjectIdentifier instead

## See Also

### Deprecated

func prepare(using: PaymentCardReader.Token, updateHandler: ((PaymentCardReader.UpdateEvent) -> Void)?) async throws -> PaymentCardReaderSession

Configures the pipeline for reading payment or loyalty cards.

Deprecated

enum UpdateEvent

An event you receive during the configuration of the payment system.

Deprecated

