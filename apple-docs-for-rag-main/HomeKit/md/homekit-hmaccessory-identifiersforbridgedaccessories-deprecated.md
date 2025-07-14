

- HomeKit
- HMAccessory
-  identifiersForBridgedAccessories Deprecated

Instance Property

# identifiersForBridgedAccessories

An array of identifiers for accessories available through a bridge.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var identifiersForBridgedAccessories: [UUID]? { get }
```

Deprecated

Use uniqueIdentifiersForBridgedAccessories instead.

## Discussion

This value is `nil` for accessories that are not bridges.

## See Also

### Managing bridged accessories

var isBridged: Bool

A Boolean that indicates whether the accessory is accessed through a bridge.

var uniqueIdentifiersForBridgedAccessories: [UUID]?

An array of unique identifiers, each of which represents an accessory vended by the bridge.

