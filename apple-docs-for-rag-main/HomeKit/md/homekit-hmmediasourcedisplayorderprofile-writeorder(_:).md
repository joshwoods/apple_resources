

- HomeKit
- HMMediaSourceDisplayOrderProfile
-  writeOrder(\_:) 

Instance Method

# writeOrder(\_:)

Writes the display order of the media sources to the accessory.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func writeOrder(_ order: [Int]) async throws
```

## Parameters 

`order`  

The new display order for the media sources. Provides an ordered list of HMCharacteristicTypeIdentifier values for HMServiceTypeInputSource services associated with the profile.

## Discussion

An error is thrown if the source ordering fails to be written to the accessory.

## See Also

### Managing input source order

var delegate: (any HMMediaSourceDisplayOrderProfile.Delegate)?

The property that handles updates to the display order.

var order: [Int]

The display order of input media sources.

let canModifyOrder: Bool

A Boolean that indicates if the display order of the input media sources can be modified.

protocol Delegate

The protocol through which a delegate receives updates on the order of input media sources.

