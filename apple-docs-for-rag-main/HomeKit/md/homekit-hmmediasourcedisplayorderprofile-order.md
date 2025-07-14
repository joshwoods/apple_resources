

- HomeKit
- HMMediaSourceDisplayOrderProfile
-  order 

Instance Property

# order

The display order of input media sources.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var order: [Int] { get }
```

## Discussion

Provides an ordered list of HMCharacteristicTypeIdentifier values for HMServiceTypeInputSource services associated with the profile.

## See Also

### Managing input source order

func writeOrder([Int]) async throws

Writes the display order of the media sources to the accessory.

var delegate: (any HMMediaSourceDisplayOrderProfile.Delegate)?

The property that handles updates to the display order.

let canModifyOrder: Bool

A Boolean that indicates if the display order of the input media sources can be modified.

protocol Delegate

The protocol through which a delegate receives updates on the order of input media sources.

