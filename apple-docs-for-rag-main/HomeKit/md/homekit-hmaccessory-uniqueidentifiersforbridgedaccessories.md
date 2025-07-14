

- HomeKit
- HMAccessory
-  uniqueIdentifiersForBridgedAccessories 

Instance Property

# uniqueIdentifiersForBridgedAccessories

An array of unique identifiers, each of which represents an accessory vended by the bridge.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var uniqueIdentifiersForBridgedAccessories: [UUID]? { get }
```

## Discussion

This value is `nil` for accessories that aren’t bridges. See the isBridged property for more information about working with bridges.

## See Also

### Managing bridged accessories

var isBridged: Bool

A Boolean that indicates whether the accessory is accessed through a bridge.

var identifiersForBridgedAccessories: [UUID]?

An array of identifiers for accessories available through a bridge.

Deprecated

