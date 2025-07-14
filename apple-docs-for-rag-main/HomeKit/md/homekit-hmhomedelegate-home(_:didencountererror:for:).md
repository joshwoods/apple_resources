

- HomeKit
- HMHomeDelegate
-  home(\_:didEncounterError:for:) 

Instance Method

# home(\_:didEncounterError:for:)

Tells the delegate that a configured accessory encountered an error.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func home(
    _ home: HMHome,
    didEncounterError error: any Error,
    for accessory: HMAccessory
)
```

## Parameters 

`home`  

The home.

`error`  

The error encountered by the accessory.

`accessory`  

The accessory that encountered the error.

## Discussion

The delegate should check whether the accessory is blocked.

## See Also

### Observing Accessories

func home(HMHome, didUnblockAccessory: HMAccessory)

Tells the delegate that an accessory has been unblocked.

