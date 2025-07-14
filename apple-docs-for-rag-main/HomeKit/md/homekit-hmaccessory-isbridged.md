

- HomeKit
- HMAccessory
-  isBridged 

Instance Property

# isBridged

A Boolean that indicates whether the accessory is accessed through a bridge.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var isBridged: Bool { get }
```

## Discussion

A bridge is a special type of accessory that allows you to communicate with accessories that can’t communicate directly with HomeKit. For example, a bridge might be a hub for multiple lights that use a communication protocol other than HomeKit Accessory Protocol.

Bridged accessories have the isBridged property set to true and depend on the bridge to communicate with HomeKit. All other accessories, including the bridge itself, have an isBridged property setting of false.

To add a bridge to a home, use the home’s addAndSetupAccessories(completionHandler:) method, as you would for any other accessory. The accessories behind the bridge are automatically added to the home as well. The home’s delegate doesn’t receive a home(_:didAdd:) delegate message for the bridge, but does receive one for each accessory behind the bridge.

When you add a bridge to a room, the accessories behind the bridge are not automatically added to the room because the bridge and its accessories might be located in different rooms. Manage each accessory’s room independently.

If you remove a bridge from the home, all of its accessories are also removed. On the other hand, you can’t directly remove a bridged accessory from the home. You can only remove the bridge.

In all other respects, you treat the accessories behind a bridge in the same way as any other accessory in a home. They appear in the home’s accessories array like non-bridged accessories, and respond to all the same commands.

## See Also

### Managing bridged accessories

var uniqueIdentifiersForBridgedAccessories: [UUID]?

An array of unique identifiers, each of which represents an accessory vended by the bridge.

var identifiersForBridgedAccessories: [UUID]?

An array of identifiers for accessories available through a bridge.

Deprecated

