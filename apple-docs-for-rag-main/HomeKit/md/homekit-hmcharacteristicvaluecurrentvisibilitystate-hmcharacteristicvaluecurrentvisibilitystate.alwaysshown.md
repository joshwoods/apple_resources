

- HomeKit
- HMCharacteristicValueCurrentVisibilityState
-  HMCharacteristicValueCurrentVisibilityState.alwaysShown 

Case

# HMCharacteristicValueCurrentVisibilityState.alwaysShown

The media source is always displayed.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
case alwaysShown
```

## Discussion

The media source can’t be hidden by writing to its Target Visibility State characteristic, even if one is included.

## See Also

### Visibility states

case connected

The media source is displayed since there’s a device connected to the input source.

case hidden

The media source isn’t displayed.

case shown

The media source is displayed.

