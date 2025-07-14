

- HomeKit
- HMAccessory
-  identifier Deprecated

Instance Property

# identifier

A unique identifier for the accessory.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var identifier: UUID { get }
```

Deprecated

Use uniqueIdentifier instead.

## Discussion

An identifier is stable for as long as an accessory is in a home. If an accessory is removed from a home, it will get a new identifier when it is next added to a home.

## See Also

### Identifying an Accessory

var name: String

The name of the accessory.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Changes the name of the accessory.

var uniqueIdentifier: UUID

A unique identifier for the accessory.

