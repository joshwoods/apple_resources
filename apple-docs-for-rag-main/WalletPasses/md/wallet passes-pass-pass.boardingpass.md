

- Wallet Passes
- Pass
-  Pass.BoardingPass 

Object

# Pass.BoardingPass

An object that represents the groups of fields that display the information for a boarding pass.

iOS 6.0+iPadOS 6.0+watchOS 2.0+

``` source
object Pass.BoardingPass
```

## Properties

`transitType`

`string`

 (Required) 

The type of transit for a boarding pass. This key is invalid for other types of passes.

The system may use the value to display more information, such as showing an airplane icon for the pass on watchOS when the value is set to `PKTransitTypeAir`.

Possible Values: `PKTransitTypeAir, PKTransitTypeBoat, PKTransitTypeBus, PKTransitTypeGeneric, PKTransitTypeTrain`

## Relationships

### Inherits From

- PassFields

## See Also

### Setting the pass type

object Pass.Coupon

An object that represents the groups of fields that display the information for a coupon.

object Pass.EventTicket

An object that represents the groups of fields that display the information for an event ticket.

object Pass.Generic

An object that represents the groups of fields that display the information for a generic pass.

