

- AVFoundation
- AVPlayerMediaSelectionCriteria
-  principalMediaCharacteristics 

Instance Property

# principalMediaCharacteristics

An array of media characteristics that are essential to select when choosing media with a particular characteristic.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var principalMediaCharacteristics: [AVMediaCharacteristic]? { get }
```

## Discussion

If no option matches the principal media characteristics, the system chooses the default option in the group as the best match.

When making automatic selections, a player item treats principal media characteristics as criteria that supersede language preferences and preferred media characteristics.

Important

Use principal media characteristics with caution. It’s typical to support accessibility features using a combination of language preferences and preferred characteristics, and not using principal media characteristics.

## See Also

### Retrieving Selection Criteria Settings

var preferredLanguages: [String]?

An array of language identifiers in preferred order.

var preferredMediaCharacteristics: [AVMediaCharacteristic]?

An array of media characteristics in preferred order.

