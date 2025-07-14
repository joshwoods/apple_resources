

- HomeKit
- HMHomeDelegate
-  home(\_:didUnblockAccessory:) 

Instance Method

# home(\_:didUnblockAccessory:)

Tells the delegate that an accessory has been unblocked.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func home(
    _ home: HMHome,
    didUnblockAccessory accessory: HMAccessory
)
```

## Parameters 

`home`  

The home.

`accessory`  

The accessory that was unblocked.

## See Also

### Observing Accessories

func home(HMHome, didEncounterError: any Error, for: HMAccessory)

Tells the delegate that a configured accessory encountered an error.

