

- ProximityReader
- PaymentCardReaderSession
- PaymentCardReaderSession.Event
-  hashValue Deprecated

Instance Property

# hashValue

The hash value.

iOS 15.4–16.0DeprecatediPadOS 15.4–16.0DeprecatedMac Catalyst 17.0–17.0Deprecated

``` source
var hashValue: Int { get }
```

Deprecated

Use PaymentCardReader.Event

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

