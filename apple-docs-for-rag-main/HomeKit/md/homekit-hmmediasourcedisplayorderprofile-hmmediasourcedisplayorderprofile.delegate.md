

- HomeKit
- HMMediaSourceDisplayOrderProfile
-  HMMediaSourceDisplayOrderProfile.Delegate 

Protocol

# HMMediaSourceDisplayOrderProfile.Delegate

The protocol through which a delegate receives updates on the order of input media sources.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol Delegate : AnyObject, Sendable
```

## Topics

### Instance Methods

func mediaSourceDisplayOrderProfileDidUpdateOrder(HMMediaSourceDisplayOrderProfile)

Informs the delegate when the system modifies the media source display order.

**Required**

## Relationships

### Inherits From

- Sendable

## See Also

### Managing input source order

func writeOrder([Int]) async throws

Writes the display order of the media sources to the accessory.

var delegate: (any HMMediaSourceDisplayOrderProfile.Delegate)?

The property that handles updates to the display order.

var order: [Int]

The display order of input media sources.

let canModifyOrder: Bool

A Boolean that indicates if the display order of the input media sources can be modified.

