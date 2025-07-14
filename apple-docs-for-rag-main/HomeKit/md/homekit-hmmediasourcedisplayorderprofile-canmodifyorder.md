

- HomeKit
- HMMediaSourceDisplayOrderProfile
-  canModifyOrder 

Instance Property

# canModifyOrder

A Boolean that indicates if the display order of the input media sources can be modified.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
final let canModifyOrder: Bool
```

## See Also

### Managing input source order

func writeOrder([Int]) async throws

Writes the display order of the media sources to the accessory.

var delegate: (any HMMediaSourceDisplayOrderProfile.Delegate)?

The property that handles updates to the display order.

var order: [Int]

The display order of input media sources.

protocol Delegate

The protocol through which a delegate receives updates on the order of input media sources.

